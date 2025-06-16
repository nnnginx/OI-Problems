<p>
For each prefix of a given string <b><i>S </i></b>with <b><i>N </i></b>characters (each character has an ASCII code between 97 and 126, inclusive), we want to know whether the prefix is a periodic string. That is, for each <b><i>i </i></b>(2 &lt;= <b><i>i </i></b> &lt;= <b><i>N</i></b>) we want to know the largest <b><i>K </i></b>&gt; 1 (if there is one) such that the prefix of <b><i>S </i></b>with length <b><i>i </i></b>can be written as <b><i>A</i><sup><i>K </i></sup></b>, that is <b><i>A </i></b>concatenated <b><i>K </i></b>times, for some string <b><i>A</i></b>. Of course, we also want to know the period <b><i>K</i></b>.
</p>

<h3>Input</h3>
<p>
The first line of the input file will
contains only the number <i>T (1 &lt;= T &lt;= 10) </i> of the test cases.
</p>
<p>
Each test case consists of two
lines. The first one contains <b><i>N</i></b> (2 &lt;= <b><i>N</i></b> &lt;= 1 000 000) ¨C the size of the string <b><i>S</i></b>.
The second line contains the string <b><i>S</i></b>.
</p>

<h3>Output</h3>
<p>
For each test case, output ¡°Test case #¡± and the consecutive test case
number on a single line; then, for each prefix with length <b>i</b> that has a period <b>K</b> &gt; 1, output the prefix size <b>i</b> and the period <b>K</b> separated by a single space; the
prefix sizes must be in increasing order. Print a blank line after each test case.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
3
aaa
12
aabaabaabaab

<b>Output:</b>
Test case #1
2 2
3 3

Test case #2
2 2
6 2
9 3
12 4

</pre>