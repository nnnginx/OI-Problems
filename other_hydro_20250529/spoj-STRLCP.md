<p>The LCP (Longest Common Prefix) of two strings A[1..la] and B[1..lb] is defined as follows:
<br><br>
LCP(A[1..la],B[1..lb]) = max{L | L&lt;=la &amp;&amp; L&lt;=lb &amp;&amp; A[1..L] == B[1..L]}
<br><br>
Given an original string and several operations, you should write a program to process all the operations.

</p><h3>Input</h3>
<p>The first line will be number of test cases T.<br>
The first line of each test case is a string S with length L (1 &lt;= L &lt;= 100000).<br>
The second line contains an integer Q(1 &lt;= Q &lt;= 150000), representing the number of operations.<br><br>
Each of the following Q lines represents an operation:<br>
Q i j: print LCP(S[i..L], S[j..L])<br>
R i char: replace the i-th character of S with char<br>
I i char: insert character char after the i-th character of S<br>

</p><h3>Output</h3>
<p>For each "Q i j" operation, print the answer.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
madamimadam
7
Q 1 7
Q 4 8
Q 10 11
R 3 a
Q 1 7
I 10 a
Q 2 11

<b>Output:</b>
5
1
0
2
1
</pre>