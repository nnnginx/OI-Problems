<p>You're given a sequence A of N non-negative integers. Answer Q queries, where each query consists of three integers: v, a, b. The answer is number of pairs of integers i and j that satisfy these conditions:
</p><p>1 &lt;= i &lt;= j &lt;= N
</p><p>a &lt;= j-i+1 &lt;= b
</p><p>A[k] &gt;= v for every integer k between i and j, inclusive
</p><h3>Constraints</h3>
<p>1 &lt;= N &lt;= 100 000
</p><p>1 &lt;= Q &lt;= 100 000
</p><p>0 &lt;= A[k] &lt;= 1000, for every integer k between 1 and N, inclusive
</p><p>0 &lt;= v &lt;= 1000
</p><p>1 &lt;= a &lt;= 100 000
</p><p>1 &lt;= b &lt;= 100 000


</p><h3>Input</h3>
<p>The first line of input contains two integers, N and Q. The second line contains the sequence A, consisting of N integers. Each of the next Q lines contains three numbers, v, a and b, defining a query.

</p><h3>Output</h3>
<p>In the i-th line output only one integer denoting the answer to the i-th query.

</p><h3>Example</h3>

<pre><b>Input:</b>
5 3
5 3 2 7 4
3 2 3
2 2 5
4 1 1

<b>Output:</b>
2
10
3
</pre>