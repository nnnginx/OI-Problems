<p>
Let's consider the alphabet consisting of the first <b>c</b> roman uppercase letters, i.e. {A, B, C, D, E, F} if <b>c</b> is 6.
<br>
We will call two words <i>quite different</i>, if there is no common subsequence of length more than one between those two words. For example ABC and CBA are quite different, but ABBA and CADDCAD aren't, because AA is a subsequence of both words.
<br>
Given a word <b>w</b> you are to find the number of words of length <b>n</b> that are quite different from <b>w</b>.

</p><h3>Input</h3>
<p>
The first line will contain the number of test cases (at most 20). Then there will be pairs of lines, the first one containing the numbers <b>n</b> (<b>n</b> will fit into a 32-bit signed integer and will be non-negative) and <b>c</b> (1 &lt;= <b>c</b> &lt;= 6), the second one the word <b>w</b>. <b>w</b> will only consist of the first <b>c</b> letters of the roman alphabet and will have at most 10000 characters.

</p><h3>Output</h3>
<p>
Print one line for each test case, consisting only of the number of words that are quite different from <b>w</b>. As this number can be quite large, you just have to output its remainder when dividing by 4242.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
3 3
ABC
4 4
CADDCAD
100 3
A

<b>Output:</b>
10
13
2223

</pre>