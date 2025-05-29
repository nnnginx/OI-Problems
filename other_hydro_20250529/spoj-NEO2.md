<p>Given array with n integer elements. We divide it into several part (may be 1), each part is a consecutive of elements. The <strong>NEO value</strong> in that case is computed by: Sum of value of each <strong>part</strong>. Value of a <strong>part</strong> is sum all elements in this part multiple by its length.</p>
<p><strong>Example:</strong> We have array: [ 2 3 -2 1 ]. If we divide it look likes: [2 3] [-2 1]. Then NEO = (2 + 3) * 2 + (-2 + 1) * 2 = 10 - 2 = 8.</p>
<p>Because there are many ways to divide an array into several part, so we can get many of NEO value. Your task is find the NEO with maximum value.</p>
<h3>Input</h3>
<p>First line: T (number of test case, T &lt;= 10)</p>
<p>For each of testcase:</p>
<p>+ First line: n (1 &lt;= n &lt;= 10^5)</p>
<p>+ Second line: a[1], a[2], ..., a[n] (-10^6 &lt;= a[i] &lt;= 10^6)</p>
<h3>Output</h3>
<p>Each testcase print the</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1<br>4
1 2 -4 1<br>
<strong>Output:</strong>
3
</pre>