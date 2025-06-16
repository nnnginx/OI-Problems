<p>You have given a matrix of size nxm. Every cell of matrix denote gcd of respective indices. For ex-</p>
<p>A 3x2 matrix have entries</p>

<table border="0">
<tbody>
<tr>
<td>gcd(1,1)&nbsp;</td>
<td>&nbsp;gcd(1,2)</td>
</tr>
<tr>
<td>gcd(2,1)</td>
<td>&nbsp;gcd(2,2)</td>
</tr>
<tr>
<td>gcd(3,1)</td>
<td>&nbsp;gcd(3,2)</td>
</tr>
</tbody>
</table>

<p>&nbsp;</p>
<p>You have given queries i1 j1 i2 j2.</p>
<p>You have to find the sum of matrix formed by upper left corner (i1,j1) and lower right corner (i2,j2).</p>

<h3>Input</h3>
<p>First line indicates number of testcases. (T&lt;=50000)</p>
<p>Next line have space separated two integer n and m. (1&lt;=n,m&lt;=1000000).</p>
<p>Next T lines contains queries i1 j1 i2 j2.&nbsp;</p>
<p>where i1&lt;=i2 j1&lt;=j2.</p>

<h3>Output</h3>
<p>Print ans modulo M for each query in newline. (M=10^9+7)</p>
<h3>Example</h3>

<pre><strong>Input:</strong>
2
3 2
1 1 2 2
2 1 3 2

<strong>Output:</strong>
5
5</pre>