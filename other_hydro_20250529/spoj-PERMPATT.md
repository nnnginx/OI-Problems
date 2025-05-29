<p>Given a permutation P[1...n] of {1,2,...n}, you should output if the permutation contains a pattern of the form 1324. That is, do there exist indices &nbsp;1 &lt;= i1 &lt; i2 &lt; i3 &lt; i4 &lt;= n such that &nbsp;P[i1] &lt; P[i3] &lt; P[i2] &lt; P[i4]. For example, P = 6 8 5 4 9 3 7 2 1 10 contains one: the indices 1, 2, 7, 10 correspond to the sequence &nbsp;6 8 7 10 which is a 1324 pattern.</p>
<h3>Input</h3>
<p>First line contains T, the number of test cases</p>
<p>Each of the next T lines contains <strong>n </strong>(1 &lt;= n &lt;= 100000), followed by <strong>n</strong>&nbsp;integers, representing a permutation of [1,2,..,n].</p>
<p>SUM( n * log<sub>2</sub>(n)) over all test cases &lt;= 10<sup>8</sup>. Do not assume anything else about the number of test cases or their distribution.</p>
<h3>Output</h3>
<p>Output T lines, one per test case: "yes"(without quotes) if the permutation contains a 1324 pattern or "no" (without quotes) otherwise.</p>
<p><strong>Warning: </strong>Huge I/O</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
10 6 8 5 4 9 3 7 2 1 10
10 5 3 4 7 9 10 8 6 2 1

<strong>Output:</strong>
yes
no</pre>