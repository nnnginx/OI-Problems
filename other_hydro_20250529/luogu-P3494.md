## 题目描述
The Byteotian Institute of Telecommunication (BIT) sets standards for data transmission in telecommunication networks all over Byteotia.

Byteasar, one of the engineers employed at BIT, works on prefix codes - a certain way of representing characters.

For each and every character of the Byteotian alphabet there is a corresponding sequence of bits, called the code word of that character.

The code words of all characters have the following properties:

None of the code words is a prefix (i.e. a leading       fragment) of another code word.

For example, if 010010 is the code word of the letter   A, then neither the bit sequence 0,   01, 010,  0100 nor 01001   is a code word of another letter.

Likewise, 0100100, 0100101 and longer   sequences starting with 010010 are not code words.

If a given bit sequence ![](http://main.edu.pl/images/OI16/kod-en-tex.1.png) is a prefix of another code word,       but not the complete code, then each of the bit sequences       ![](http://main.edu.pl/images/OI16/kod-en-tex.2.png) and ![](http://main.edu.pl/images/OI16/kod-en-tex.3.png) (that is, ![](http://main.edu.pl/images/OI16/kod-en-tex.4.png) with zero or one       appended at the end) is a prefix of some code word, or the       complete code word.

For example, if 0100 is the prefix of the code word of the       letter A, then 01000 and 01001 each       is a prefix of some code word, or a complete code word.

Let us consider the following exemplary prefix code for the alphabet consisting of the characters    A, B, C, D and E:

charactercode word    A00    B10    C11    D010    E011         Encoding a sequence of characters with a prefix code consists in concatenating the code words of its successive characters.

For example, the encoding of the sequence BACAEBABAE is 1000110001110001000011.

Byteasar noticed that if some leading bits are lost, the sequence may be decoded wrong, or it may even be not decoded at all.

For example, if five initial bits of the sequence given above are removed, the resulting sequence 10001110001000011 will be decoded as BACBABAE.

The last five letter (BABAE) are correct, but the first three (BAC) are not.

Byteasar further noticed that all the letters after the first E are decoded correct.

He concluded that whenever all the bits of the code word of E are intact, all the characters succeeding E will be decoded correct.

The same holds for every encoded sequence obtained from one that contains E.

He also noticed that the letter D shares this feature, but A, B and C do not.

Because of the properties of the code words of E and D Byteasar called them synchronising code words.

He trusted you with the task of writing a programme that finds all the synchronising code words of a given prefix code.

To save some time, he intends to present you all the code words on his binary monitor.

This interesting device has four buttons:

0 - append ![](http://main.edu.pl/im…


## 输入格式
In the first line of the standard input there is an integer ![](http://main.edu.pl/images/OI16/kod-en-tex.7.png)      (![](http://main.edu.pl/images/OI16/kod-en-tex.8.png)) denoting the number of buttons pressed      by Byteasar.

In the following line an ![](http://main.edu.pl/images/OI16/kod-en-tex.9.png) letters long string consisting of the      characters '0', '1', 'B' and      'X' is given; the characters correspond to the buttons,      of course.

Each time the button X is pressed, a code word is      completed and another one starts.

The code words are numbered starting with 1.

The sum of lengths of all code words will not exceed ![](http://main.edu.pl/images/OI16/kod-en-tex.10.png).


## 输出格式
The number ![](http://main.edu.pl/images/OI16/kod-en-tex.11.png) of synchronising code words should be printed out in the     first line of the standard output.

The following ![](http://main.edu.pl/images/OI16/kod-en-tex.12.png) lines should contain the numbers of code words that  are synchronising in increasing order, each in a separate line.

If the given prefix code contains no synchronising code words, the first  line should contain the number 0, and no more lines should follow.


## 题目大意
## 题面翻译

有若干个字符，对于每一个，用一个 $01$ 串编码它。所有的 $01$ 串由一棵完全的 trie (每个点有两个儿子)给出(具体方式见输入格式)，保证有且仅有每个叶子对应一个字符。定义一个串 $s$ 编码的结果是其中各个字符的编码按顺序接起来，记为 $\mathrm{encode}(s)$。

定义对一个 $01$ 串进行解码的过程是，每次找到一个前缀，满足它对应一个字符，容易知道这样的前缀是唯一的。将这个字符加入答案，将这个前缀从原串中删掉，如果不存在这样的前缀，则解码的结果是未定义。记 $s$ 解码的结果是 $\mathrm{decode}(s)$。

设一个字符编码为 $a$，定义它是好的，当且仅当对于任意两个串 $s,t$，对于 $\mathrm{encode}(s)$ 的任意后缀 $p$，有 $\mathrm{decode}(p+a)$ 不是未定义，且 $\mathrm{decode}(p+a+\mathrm{encode}(t))=\mathrm{decode}(p+a)+t$。求哪些字符是好的。

## 输入格式

第一行一个数 $n$，表示操作次数。接下来一行一个长 $n$ 的字符串，其中 `0`/`1` 表示在当前结点添加一个儿子，边权为 `0`/`1`，并移动过去；`B`表示添加一个父亲；`X`表示当前结点是一个字符的编码。保证输入是描述这棵 trie 的最短的可能输入。$n\leq 3\times 10^6$ ，所有字符编码的总长 $\leq 10^8$ 。

## 输出格式

一行一个数，表示好的字符的数量。

接下来若干行，从小到大输出每个好的字符是第几个`X`生成的。



```input1
21
11XB0XBB00XB11XB0XBBB

```

```output1
2
4
5

```

