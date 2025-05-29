<p></p><p>
Bruce Force has had an interesting idea how to encode strings.
The following is the description of how the encoding is done:
</p>
<p>
Let x<sub>1</sub>,x<sub>2</sub>,...,x<sub><i>n</i></sub> be the sequence of characters of the string to be encoded.
</p><ol>
<li>Choose an integer <i>m</i> and <i>n</i> pairwise distinct numbers p<sub>1</sub>,p<sub>2</sub>,...,p<sub><i>n</i></sub> from the set {<i>1</i>, <i>2</i>, ..., <i>n</i>}
(a permutation of the numbers <i>1</i> to <i>n</i>).

</li><li>Repeat the following step <i>m</i> times.</li>
<li>For <i>1</i> �� i �� <i>n</i> set y<sub>i</sub> to x<sub>p<sub>i</sub></sub>, and then for <i>1</i> �� i �� <i>n</i> replace x<sub>i</sub> by y<sub>i</sub>.

</li></ol>
<p>
For example, when we want to encode the string "hello", and we choose the value <i>m = 3</i>
and the permutation <i>2, 3, 1, 5, 4</i>, the data would be encoded in 3 steps:
"hello" -&gt; "elhol" -&gt; "lhelo" -&gt; "helol".
</p>
<p>
Bruce gives you the encoded strings, and the numbers <i>m</i> and p<sub>1</sub>, ..., p<sub><i>n</i></sub> used to encode these strings.
He claims that because he used huge numbers <i>m</i> for encoding, you will need a lot of time to decode the strings.
Can you disprove this claim by quickly decoding the strings?
</p>

<h3>Input</h3>
<p>The input contains several test cases.
Each test case starts with a line containing two numbers <i>n</i> and <i>m</i> (<i>1 �� n �� 80</i>, <i>1 �� m �� 10<sup>9</sup></i>).
The following line consists of <i>n</i> pairwise different numbers p<sub>1</sub>,...,p<sub><i>n</i></sub> (<i>1</i> �� p<sub>i</sub> �� <i>n</i>).
The third line of each test case consists of exactly <i>n</i> characters, and represent the encoded string.
The last test case is followed by a line containing two zeros.
</p>
<h3>Output</h3>
<p>For each test case, print one line with the decoded string.
</p>
<h3>Example</h3>

<pre><b>Input:</b>
5 3
2 3 1 5 4
helol
16 804289384
13 10 2 7 8 1 16 12 15 6 5 14 3 4 11 9
scssoet tcaede n
8 12
5 3 4 2 1 8 6 7
encoded?
0 0

<b>Output:</b>
hello
second test case
encoded?
</pre>