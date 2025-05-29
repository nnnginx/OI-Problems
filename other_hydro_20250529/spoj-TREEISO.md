<p>Given two undirected trees T1 and T2 with equal number of vertices N (1 ¡Ü N ¡Ü 100,000) numbered 1 to N, find out if they are isomorphic.<br><br>Two trees T1 and T2 are isomorphic if there is a bijection f between the vertex sets of T1 and T2 such that any two vertices u and v of T1 are adjacent in T1 if and only if f(u) and f(v) are adjacent in T2.</p>
<h3>Input</h3>
<p>The first line of input contains the number of test cases nTest (1&lt;= nTest &lt;= 400). Each test case contains:</p>
<ul>
<li>The first line contains the number of nodes N.</li>
<li>Each of next N-1 lines contain two integers A, B, denoting that there is an edge in T1 between nodes A and B (1 ¡Ü A, B ¡Ü N).</li>
<li>Each of next N-1 lines contain two integers A, B, denoting that there is an edge in T2 between nodes A and B (1 ¡Ü A, B ¡Ü N).</li>
</ul>
<p>The sum of N over all test cases will not exceed 100,000.</p>
<h3>Output</h3>
<p>For each test case print YES if T1 and T2 are isomorphic and NO otherwise.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2<br>4<br>4 2<br>4 1<br>2 3<br>4 2<br>2 3<br>4 1<br>5<br>3 4<br>3 2<br>3 5<br>3 1<br>3 4<br>4 2<br>2 5<br>2 1

<strong>Output:</strong>
YES<br>NO
</pre>