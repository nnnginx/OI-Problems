<p>Antique Comedians of Malidinesia would like to play a new discovered
comedy of Aristofanes. Putting it on a stage should be a big surprise for
the audience so all the preparations must be kept absolutely secret.
The ACM director suspects one of his competitors of reading his
correspondece. To prevent other companies from revealing his secret, he
decided to use a substitution cipher in all the letters mentioning the
new play.

</p><p>Substitution cipher is defined by a substitution table assigning each
character of the substitution alphabet another character of the same alphabet.
The assignment is a bijection (to each character exactly
one character is assigned -- not neccessary different).
The director is afraid of disclosing the substitution table and
therefore he changes it frequently. After each change he chooses a few
words from a dictionary by random, encrypts them and sends them together with
an encrypted message. The plain (i.e. non-encrypted) words
are sent by a secure channel, not by mail. The recipient of the message
can then compare plain and encrypted words and create
a new substitution table.

</p><p>Unfortunately, one of the ACM cipher specialists have found that this
system is sometimes insecure. Some messages can be decrypted by the rival
company even without knowing the plain words. The reason is
that when the director chooses the words from the dictionary and encrypts them, 
he never changes their order (the words in the dictionary are
lexicographically sorted). String <var>a<sub>1</sub>a<sub>2</sub> ...
a<sub>p</sub></var> is lexicografically smaller than
<var>b<sub>1</sub>b<sub>2</sub> ... b<sub>q</sub></var> if there exists an
integer <var>i</var>, <var>i &lt;= p, i &lt;= q</var>, such that
<var>a<sub>j</sub>=b<sub>j</sub></var> for each <var>j, 1 &lt;= j &lt;
i</var> and <var>a<sub>i</sub> &lt; b<sub>i</sub></var>.

</p><p>The director is interested in which of his messages could be
read by the rival company. You are to write a program to determine that.


</p><h3>Input</h3>

<p>The input consists of <var>N</var> cases (equal to about 1000). The first line of the input
contains only positive integer <var>N</var>. Then follow the cases. 
The first line of each case contains only two positive integers
<var>A</var>, <var>1 &lt;= A &lt;= 26</var>, and <var>K</var>, separated by
space. <var>A</var> determines the size of the substitution alphabet (the
substitution alphabet consists of the first <var>A</var> lowercase letters
of the english alphabet (a--z) and <var>K</var> is the number of encrypted
words. The plain words contain only the letters of the substitution
alphabet. The plain message can contain any symbol, but only the letters of
the substitution alphabet are encrypted. Then follow <var>K</var> lines,
each containing exactly one encrypted word. At the next line is encrypted
message.


</p><h3>Output</h3>

<p>For each case, print exactly one line. If it is possible
to decrypt the message uniquely, print the
decrypted message. Otherwise, print the sentence
'<tt>Message cannot be decrypted.</tt>'.


</p><h3>Example</h3>
<pre>Sample input:

2
5 6
cebdbac
cac
ecd
dca
aba
bac
cedab
4 4
cca
cad
aac
bca
bdac

Sample output:

abcde
Message cannot be decrypted.
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>