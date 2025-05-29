<p>You're given a sequence A of N non-negative integers. Answer Q queries, where each query consists of two integers: a, b. The answer is number of pairs of integers i and j that satisfy these three conditions:<br><br>(1) 1 &lt;= i &lt;= j &lt;= N</p>
<p>(2) a &lt;= j-i+1 &lt;= b</p>
<p>(3) all elements of A with indices from range [i, j] are mutually distinct. (indexing starts with 1)</p>
<p><strong>Constraints</strong> :<br><br>1 &lt;= N &lt;= 8*10^5<br>1 &lt;= Q &lt;= 2*10^5<br>0 &lt;= A[k] &lt;= 10^6, for every integer k between 1 and N, inclusive<br><br>1 &lt;= a &lt;= b &lt;= N</p>
<h3>Input</h3>
<p>First line of input contains integer N. Second line contains N integers representing sequence A. Third line is integer Q, number of queries. Next Q lines have 2 integers, a and b.</p>
<h3>Output</h3>
<p>In the i-th line output the answer for i-th query.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>5<br>1 2 3 4 5<br>1<br>1 1<br><br><strong>Output:</strong><br><br>5<br><br><strong>NOTE: IO is huge</strong></pre>