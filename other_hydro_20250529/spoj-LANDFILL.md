<p>You are given a sequence H[1], H[2], ... , H[N] representing the initial heights of N pieces of land and an integer K. It costs C[i] Rupees to elevate each of H[i], H[i+1], ... , H[i+K-1] by E[i]; if i+K &gt; N, it will just elevate all the pieces of land from A[i] to A[N] - Let us call this an <em>operation</em>. The following constraints must be satisfied:</p>
<p>1) For each i, the <em>operation</em>&nbsp;can be performed atmost once.</p>
<p>2) The sum of the costs of all the operations performed must be &lt;= Budget.</p>
<p>You have to calculate the maximum height V such that each plot's elevation is atleast V before you exhaust the budget.</p>
<h3>Input</h3>
<p>The first line of input contains 3 integers N, Budget and K.</p>
<p>The next N lines consists of 3 integers H[i], E[i] and C[i].</p>
<h3>Output</h3>
<p>Output a single integer V such that all the plots have atleast height V.</p>
<h3>Constraints</h3>
<p>1 &lt;= K &lt;= 11</p>
<p>1 &lt;= N &lt;= 100</p>
<p>0 &lt;= Budget, H[i], E[i], C[i] &lt;= 1000000</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 20 1</pre>
<pre>1 3 5</pre>
<pre>1 7 3</pre>
<pre>4 6 9</pre>
<pre>3 5 13

<strong>Output:</strong>
3</pre>
<pre><strong>Explanation:</strong></pre>
<p>You can raise the level of the (unit) segments 1, 2 and 3, yielding a sequence of final heights 4, 8, 10 and 3. The minimum height among these is 3.</p>