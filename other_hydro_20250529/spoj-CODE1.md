<p align="justify">
The Sarcophagus itself is locked by a secret numerical code. When somebody
wants to open it, he must know the code and set it exactly on the top of the
Sarcophagus. A very intricate mechanism then opens the cover. If an incorrect
code is entered,
the tickets inside would catch fire immediately and they would
have been lost forever. The code (consisting of up to 100 integers)
was hidden in the Alexandrian Library but unfortunately, as you probably
know, the library burned down completely.

</p><p align="justify">
But an almost unknown archaeologist has obtained a copy of the code something
during the 18th century. He
was afraid that the code could get to the ``wrong people'' so he has
encoded the numbers in a very special way. He took a random complex number
<var>B</var> that was greater (in absolute value) than any of the encoded numbers. Then
he counted the numbers as the digits of the system with basis <var>B</var>. That means
the sequence of numbers <var>a<sub>n</sub></var>,
<var>a<sub>n-1</sub></var>, ..., <var>a<sub>1</sub></var>,
<var>a<sub>0</sub></var> was encoded as the number 
<var>X = a<sub>0</sub> + a<sub>1</sub>B + a<sub>2</sub>B<sup>2</sup> + ...+
a<sub>n</sub>B<sup>n</sup></var>.

</p><p align="justify">
Your goal is to decrypt the secret code, i.e. to express a given number <var>X</var> in
the number system to the base <var>B</var>. In other words, given the
numbers <var>X</var> and <var>B</var>you are to determine the ``digit''
<var>a<sub>0</sub></var> through <var>a<sub>n</sub></var>.


</p><h3>Input</h3>

<p align="justify">The input consists of <var>T</var> test cases (equal to about 100000). The number of them (<var>T</var>) is
given on the first line of the input file. Each test case consists of one single
line containing four integer numbers <var>X<sub>r</sub></var>,
X<sub>i</sub>, <var>B<sub>r</sub></var>, <var>B<sub>i</sub></var>
(<var>|X<sub>r</sub>|,|X<sub>i</sub>| &lt;= 1000000</var>,
<var>|B<sub>r</sub>|,|B<sub>i</sub>| &lt;= 16</var>). These numbers
indicate the real and complex components of numbers <var>X</var> and <var>B</var>,
i.e. <var>X = X<sub>r</sub> + i.X<sub>i</sub></var>,
<var>B = B<sub>r</sub> + i.B<sub>i</sub></var>. <var>B</var> is the basis of
the system (<var>|B| &gt; 1</var>), <var>X</var> is the number you have to
express.


</p><h3>Output</h3>

<p align="justify">Your program must output a single line for each test case. The line should
contain the ``digits'' <var>a<sub>n</sub></var>, <var>a<sub>n-1</sub></var>,
..., <var>a<sub>1</sub></var>, <var>a<sub>0</sub></var>, separated by 
commas. The following conditions must be satisfied:
</p><div align="left">
<ul>
<li>for all <var>i</var> in <var>{0, 1, 2, ...n}</var>:
<var>0 &lt;= a<sub>i</sub> &lt; |B|</var>

</li><li>
<var>X = a<sub>0</sub> + a<sub>1</sub>B + a<sub>2</sub>B<sup>2</sup> + ...+
a<sub>n</sub>B<sup>n</sup></var>

</li><li>if <var>n &gt; 0</var> then <var>a<sub>n</sub> &lt;&gt; 0</var>

</li><li><var>n &lt;= 100</var>
</li></ul></div>

<p align="justify">If there are no numbers meeting these criteria, output the sentence
"<code>The code cannot be decrypted.</code>". If there are more possibilities,
print any of them.


</p><h3>Example</h3>

<pre>Sample Input

4
-935 2475 -11 -15
1 0 -3 -2
93 16 3 2
191 -192 11 -12

Sample output:

8,11,18
1
The code cannot be decrypted.
16,15
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>