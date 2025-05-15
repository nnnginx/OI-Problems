# Description

The Advanced Encryption Standard (AES) involves a new strong encryption algorithm. It works with three *blocks*of 128 bits. Given a message block  *p* (plaintext) and a key block  *k* , the AES encryption function *E *returns an encrypted block  *c* (ciphertext):

*c* =  *E* ( *p* ,  *k* ) .

The inverse of the AES encryption function *E *is the decryption function *D *such that

*D* (  *E* ( *p* ,  *k* ),  *k* ) =  *p* ,	 *E* (  *D* ( *c* ,  *k* ),  *k* ) = *c* .

In  *Double AES* , two independent key blocks $k_1$ and $k_2$ are used in succession, first$k_1$ , then $k_2$ :

$c_2$=  *E* (  *E* ( *p* , $k_1$ ), $k_2$).

In this task, an integer *s *is also given. Only the leftmost 4**s *bits of keys are relevant, while the other bits (the rightmost 128 minus 4**s *bits) are all zero.

You are to recover the encryption key pairs for some messages encrypted by Double AES. You are given both the plaintext *p*and the corresponding double-encrypted ciphertext $c_2$ , and the structure of the encryption keys as expressed by the integer  *s* . The AES encryption and decryption algorithms are available in a library. You must submit the recovered keys, and not a recovery program.

# Format

## Input

You are given ten problem instances in the text files named double1.in to double10.in. Each input file consists of three lines. The first line contains the integer  *s* , the second line the plaintext block  *p* , and the third line the ciphertext block $c_2$  obtained from*p*by Double AES encryption. Both blocks are written as strings of 32 hexadecimal digits (‘0’..’9’, ‘A’..’F’). The library provides a routine to convert strings of blocks. All input files are solvable.

## Output

You are to submit ten output files corresponding to the given input files. Each output file consists of three lines. The first line contains the text

#FILE double I

where I is the number of the respective input file. The second line contains the key block $k_1$ , and the third line the key block $k_2$ , such that

$c_2$=  *E* (  *E* ( *p* , $k_1$ ), $k_2$).

Both blocks must be written as strings of 32 hexadecimal digits ( ‘0’..’9’,  ‘A’..’F’). The library provides a routine to convert strings of blocks. If there are multiple solutions, you need submit only one of them.

# Samples

```input1
1
00112233445566778899AABBCCDDEEFF
6323B4A5BC16C479ED6D94F5B58FF0C2
```

```output1
#FILE double 0 A0000000000000000000000000000000 70000000000000000000000000000000
```

# Limitation

 **Library**

FreePascal library (Linux: aeslibp.p, aeslibp.ppu, aeslibp.o;

Windows: aeslibp.p, aeslibp.ppw, aeslibp.ow):

type

HexStr = String [ 32 ]; { only '0'..'9', 'A'..'F' } Block	= array [ 0..15 ] of Byte; { 128 bits }

procedure HexStrToBlock ( const hs: HexStr; var b: Block ); procedure BlockToHexStr ( const b: Block; var hs: HexStr ); procedure Encrypt ( const p, k: Block; var c: Block );

{ c = E(p,k) }

procedure Decrypt ( const c, k: Block; var p: Block );

{ p = D(c,k) }

The program aestoolp.pas illustrates how to use the FreePascal library. GNU C/C++ library (Linux and Windows: aeslibc.h, aeslibc.o):

typedef char HexStr[33]; /* '0'..'9', 'A'..'F', '\0'-terminated */

typedef unsigned char Block[16];	/* 128 bits */

void hexstr2block ( const HexStr hs, /* out-param */ Block b ); void block2hexstr ( const Block b, /* out-param */ HexStr hs );

void encrypt ( const Block p, const Block k, /* out-param */ Block c );

/* c = E(p,k) */

void decrypt ( const Block c, const Block k, /* out-param */ Block p );

/* p = D(c,k) */

The program aestoolc.c illustrates how to use the GNU C/C++ library.

**Constraints**

For the number *s *of relevant hexadecimal digits in a key it holds that 1 £  *s * £ 5. Hint: A good program can recover any keys in less than 10 seconds for any allowed input file.

 **Abstract formulation**

Given is a pair of encryption-decryption functions E, D, such that

*D (E (p,k),k ) = p *and *E (D (c,k),k ) = c,*

for all plaintext messages p, ciphertext messages c, and keys k.

The encryption algorithm is “strong”, in the sense that no better method of recovering k for given p and c = E(p,k) is known than an exhaustive search through the key space. Given ten double- encrypted pairs p, c2 = E(E(p,k1),k2), the competitors have to recover the key pairs k1, k2.

 **History**

"Rijndael" was recently selected from five candidate encryption algorithms by the National Institute of Standards and Technology (NIST) in the USA to be proposed for the new Advanced Encryption Standard (AES). It has been subjected to intense scrutiny, and currently no weaknesses are known or expected to surface any time soon. In particular, there are no known “weak” keys (in contrast to the Data Encryption Standard DES). [See [www.nist.gov/aes/]](http://www.nist.gov/aes/)

The AES can be used with 128-bit keys and messages (and also 192 and 256). In this task, the key space is artificially reduced to control the difficulty of the instances.

 **Solution**

Double encryption, as applied in this task, is known to provide much less extra security than may at first seem to be the case. If the key length is n bits for single encryption, then an exhaustive search goes through all possible 2^n^ keys. Double encryption with two independent n-bit keys may seem to correspond to encryption with a single 2n-bit key. However, the so-called “meet-in-the-middle attack” shows that it is actually no stronger than a single (n+1)-bit key. In practice, triple encryption is used (e.g. known in Triple DES). [See e.g., Bruce Schneier, Applied Cryptography, Second Edition, Wiley, 1996]

The meet-in-the-middle attack works as follows. The given plain text p is encrypted with all possible 2^n^ keys and the results are stored (one way or another) in a table. Next, the given double- encrypted ciphertext c2 is decrypted with all possible 2^n^ keys, and each result is checked against the table for a “collision”. Such a collision reveals a “double key” used for encryption.

It is possible that more than one key pair works, though extremely unlikely (you could earn some money with such key pairs :-). In this task, only one of key pair needs to be found. For the input cases selected, it can easily be checked whether the solution are unique with in the imposed constraints (as indeed they are).

Let us consider the required computational effort in some more detail. The key space can be traversed by implementing two operations

FirstKey ( var key: Block );

NextKey ( var key: Block ): Boolean;

where the return value of NextKey indicates whether key indeed had a successor.

The table needs to provide the following operations:

EmptyTable;

initialize to empty table

Store ( const msg: Block; const key: Block );

insert a message-key pair (msg,key) where msg = Encrypt(p,key) Retrieve ( const msg: Block; var found: Boolean; var key: Block );

determine whether message msg is present, and if so, with which key k such that msg = Encrypt(p,key)

A Block equality test is also needed, to verify correct retrieval. Both the Store and the Retrieve operations need to be fast, preferably in constant time (O(1)), which suggests a hashed dictionary.

Let us consider this from the task designer's viewpoint, who does not yet know all the various parameters (such speed and memory size of computer and the limits to impose). It seems reasonable to

store the relevant part of the key (say at most 4 bytes, minus 1 special value to indicate an empty entry in the dictionary), and to hash the encrypted message to a hash value in a suitable range. The message need not be stored, since it can be reconstructed from the given plaintext and the key. But if there is enough space, it can also be stored in 16 bytes. Thus, additional operations that are needed:

CompressKey ( const key: Block ): CompressedKey; (24 bit) UncompressKey ( const ck: CompressedKey; var b: Block ); HashMessage ( const b: Block ): HashValue;

Let us assume 64 MB RAM for the table (this seems reasonable on a 128 MB machine; 64MB is the minimum for smooth operation of the operating systems, and I expect at least 128 MB). This means $2 ^{26}$ bytes available for the table. With 4 = $2 ^{2}$ byte per entry, this allows for $2 ^{24}$ entries. Thus, a 24-bit hash value seems sufficient. Given the good encryption properties of AES, it should suffice to take the first 24 bits of the encrypted plaintext as hash value. We use a special out-of-range key value in the table to indicate that an entry is unoccupied. This also means that there should not be $2 ^{24}$ or more keys (otherwise, several passes need to be made: build the table for each group of $2 ^{24}$ keys, and for each

such group decrypt with ALL possible keys). What about hash collissions when storing data? We have doubled the dictionary size to include enough empty entries to get a good response time.

In the worst case (maximum key size K bits), 2^K^ store operations and retrieve operations need to be done. Each store is accompanied by an encryption, and each retrieve by a decryption. If the encrypted message itself is not stored (but only its key), then also one or more encryptions are needed to verify equality of the message string.

I do not expect that more than $10^6$ ~~ $2^{20}$ encryptions+stores can be done per second on the competition machines. Let us assume $10 ^{4}$ ~~ $2 ^{13}$ , then breaking a 24-bit key takes at most 3*$2 ^{24}$ /$2 ^{13}$ = 3*$2 ^{11}$ seconds (2 hours!), a 20-bit key takes at most 3*$2 ^{20}$ /$2 ^{13}$ = 3*$2 ^{7}$ seconds (less than 10 minutes). For $10 ^{6}$ cycles per second, breaking a 24-bit key takes 3*$2 ^{4}$ seconds (one minute!), and a 20-bit key takes 3 seconds. The brute-force approach is quadratic and under the best circumstances, breaking a 20- bit key with $10^{6}$ encryptions per second would take 3*$2 ^{20}$ seconds, or about one month!

It turns out that AES decryption is a factor two slower than encryption. Furthermore, the selected competition computer (933 MHz Pentium-III) does about 0.5e6 AES encryptions per second. For the competition, the upper bound on s was set at 5.

 **Grading**

The most important parameter is the key size s. At small key sizes, an exhaustive search over the combined key space is still feasible. The plaintext message does not matter at all, provided that the encryption algorithm is indeed “strong”. The choice of key pair needs more attention, because it

should not be too “easy” to find “accidentally”. Thus, key values near the extremes should be avoided in general. However, the competitors are free to choose how they traverse the key space, and the organizers cannot know, in general, what constitutes a bad key choice.

Note that special cases had better be avoided, such as identical first and second keys, or keys that are very close together, or keys with patterns in them (e.g. all hex-digits equal).

The ten cases that were selected for the competition have the following characteristics:

| Case | s | T | k1       | k2       | Comments                              |
| ------ | --- | --- | ---------- | ---------- | --------------------------------------- |
| ---- | - | - | -------- | -------- | --------                              |
| 1    | 1 | P | A...     | 7...     | This case is the same as the example  |
| 2    | 1 | R | C...     | 5...     | Can be solved manually with the tool  |
| 3    | 2 | P | A7...    | 6E...    | Can be solved by exhaustive search    |
| 4    | 2 | C | E1...    | 8A...    | Can be solved by exhaustive search    |
| 5    | 4 | R | A39E...  | B760...  |                                       |
| 6    | 4 | R | 893D...  | F66B...  |                                       |
| 7    | 4 | R | 9325...  | 0000...  | Extreme key at one end of key space   |
| 8    | 5 | C | CB053... | 7F0F9... |                                       |
| 9    | 5 | P | A7000... | 6E000... | Same answer as case 3                 |
| 10   | 5 | P | 59D04... | FFFFF... | Extreme key at other end of key space |

where

s	= number of relevant hexadecimal key digits (task input) T	= type of plaintext/ciphertext:

P for structured plaintext (random-looking ciphertext) C for structured ciphertext (random-looking plaintext)

R for random plaintext/ciphertext k1 = first key (task output)

k2 = second key (task output)

**Notes**

All answers can easily be verified by the interactive tool that was provided. All possible key digits 0 , .., F appear in the keys, including duplicates. Structure in the plaintext or ciphertext cannot be exploited.

Cases with s = 4 can be solved by exhaustive search, but each takes more than one hour. Because these three cases have the same plaintext, they can be attacked together with exhaustive search, to solve three cases for the price of one case plus a little bit. Even a straightforward implementation of the

meet-in-the-middle attack works in seconds.

Cases with s = 5 require a good implementation of the meet-in-the-middle search. They cannot be solved by exhaustive search within the five hours of the competition. However, case 9 has the same solution as case 3! This can be recognized by inspecting the input files.

 **Variations**

Several other formulations were considered, but rejected. For instance, instead of measuring the relevant size of a key in hexadecimal digits, it could be measured in bits. This allows for finer

variations in the level of difficulty, but is also harder to formulate, because bit order in bytes (endianness) starts to play a role. Another variation used hexadecimal strings in the interfaces of the encryption and decryption routines. The available AES encryption and decryption implementations work on 128-bit blocks. Hence, the library would need to convert on every call, thereby introducing a considerable time penalty.

The source of the library need not be secret, because knowing the encryption algorithm does not make the job easier. On the contrary, it is a waste of time to read the details of the encryption algorithm. For that reason, it was not made avaible.

The encryption/decryption algorithm does not have to be the actual AES. Using the actual AES lends the task a touch of timeliness. The AES algorithms are comparable in speed to those for DES (Data Encryption Standard). Note that the encryption method needs to offer a certain minimal amount of real security, because we do not want the competitors to break the encryption algorithm (by finding a shortcut to key recovery, rather than using a “smart” search).

We use zero-padding to reduce the key space artificially. Padding can be done either on the left or the right (either way, the increment operation on 32-bit values cannot be used to simplify traversing the key space, because the byte order in 32-bit values and the order of the hexits in a byte are not “compatible”). Alternatively, the key space can be reduced by restricting the values of (say) four nonzero bytes, or by duplicating parts of the key.

The size of the plaintext message and encrypted message can be chosen smaller (for AES, 128 bits is the minimum). Note that zero padding the plaintext does not (usually) result in a zero-padded ciphertext.

 **Aestool**

The programs aestoolp and aestoolc given to the competitors serve three purposes:

1. They show the competitors how the libraries aeslibp and aeslibc can be used.
2. They provide a simple user interface (via stdio) for the libraries aeslibp and aeslibc, enabling the competitors to play around “manually” with the library. For example, they can now easily verify the example input and output file.
3. They provide the organizers a simple means to apply a quick test to check that the library works as intended. In particular, a very simple (and limited) test is to encrypt the all-zero plaintext with the all-zero key, which should result in ciphertext:

66E94BD4EF8A2C3B884CFA59CA342B2E

Decrypting this should again yield the all-zero plaintext.

The Pascal tool starts with the following output:

Interactive Tool for Using Library aeslibp Plaintext	= 00000000000000000000000000000000

Key	= 00000000000000000000000000000000

Ciphertext = 00000000000000000000000000000000

HexStr index 12345678901234567890123456789012 (mod 10)

Block index	0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 (mod 10) P(laintext, K(ey, C(iphertext, E(ncrypt, D(ecrypt, S(wap, Q(uit?

After the ‘?’, a single letter command must be typed, followed by ‘Enter’. The known commands are the uppercase letters before each ‘(‘. The commands have the following meaning:

P(laintext:	asks for a new plaintext C(iphertext:	asks for a new ciphertext K(ey:	asks for a new key

E(ncrypt:	encrypts given plaintext under given key to ciphertext D(ecrypt:	decrypts given ciphertext under given key to plaintext S(wap:	swaps plaintext and ciphertext (simplifies chaining) Q(uit:	terminates program execution

Plaintext, ciphertext, and key can be entered using lowercase and/or uppercase characters. These blocks are automatically right-padded with zeroes.

The C version is very similar for aeaslibc. At start it prints:

Interactive Tool for Using Library aeslibc Plaintext	= 00000000000000000000000000000000

Key	= 00000000000000000000000000000000

Ciphertext = 00000000000000000000000000000000

HexStr index 01234567890123456789012345678901 (% 10)

Block index	0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 (% 10)

P(laintext, K(ey, C(iphertext, E(ncrypt, D(ecrypt, S(wap, Q(uit?

Note that HexStr indices now start at 0.

No detailed description of these programs is to the competitors, because they get the source and should be able to understand that. Furthermore, they can experiment at will, so figuring out the tools is part of the game.

 **Other development tools**

Several other tools were developed to support the design of the task. These were

dblgen: a generator of input files given some parameters dblifv: an input file format validator

dblofv: an output file format validator

dblchk: a simple output file checker (against given input file) double-checker: a robust output file checker (using RobIn, my

Robust Input module)

And, of course, various solution programs in Pascal and C, and dozens of output files with all kinds of funny things in them to test the entire system.

