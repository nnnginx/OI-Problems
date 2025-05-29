<p>You are given sequence A of N integers. You are also given integer K and M queries. Each query consists of two integers l, r. For each query output number of pairs i, j such that l &lt;= i &lt; j &lt;= r and abs(A[i] - A[j]) &gt;= K.</p>
<p>Indexing starts with 1.</p>
<p>N &lt;= 50000</p>
<p>M &lt;= 50000</p>
<p>1 &lt;= A[i] &lt;= 100000</p>
<p>&nbsp;</p>
<p>NOTE: All tests are randomly generated.</p>
<h3>Input</h3>
<p>First line of input contains integers N, M, K in this order.</p>
<p>Second line contains N integers representing array A.</p>
<p>Next M lines describe queries.</p>
<h3>Output</h3>
<p>Output answer for each query.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 1 2<br>1 2 3<br>1 3<br><strong>Output:</strong>
1</pre>