<p>
Let us define:
</p><ul>
  <li>F[1] = 1</li>
  <li>F[i] = (a*M[i] + b*i + c)%1000000007 for i &gt; 1</li>
</ul>
<p>where M[i] is the median of the array {F[1], F[2], ..., F[i-1]}.</p>

<p>The median of an array is the middle element of that array when it is sorted. If there are an even number of elements in the array, we choose the first of the middle two elements to be the median.</p>

<p>Given a, b, c and n, calculate the sum F[1] + F[2] + .. + F[n].</p>

<h3>Input</h3>
<p>The first line contains T the number of test cases. Each of the next T lines contain 4 integers : a, b, c and n.</p>

<h3>Output</h3>
<p>Output T lines, one for each test case, containing the required sum.</p>

<h3>Constraints</h3>
<p>1 &lt;= T &lt;= 100<br>
0 &lt;= a, b, c &lt; 1000000007<br>
1 &lt;= n &lt;= 200000</p>

<h3>Example</h3>
<p>Sample Input:</p>
<pre>2
1 0 0 3
3 1 2 6</pre>

<p>Sample Output:</p>
<pre>3
103</pre>