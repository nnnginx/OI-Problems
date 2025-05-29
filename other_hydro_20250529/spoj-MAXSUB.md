<p>Given an array find the sum of the maximum non-empty subset of the array and also give the count of the subset. A subset of an array is a list obtained by striking off some (possibly none) numbers.</p>
<p>A non-empty subset implies a subset with at least 1 element in it.</p>

<h3>Input</h3>
<p>First line contains an integer T which is the number of integers. Following this T-cases exist.</p>
<p>Each case starts with a line containing an integer n which is the number of elements in the array.</p>
<p>The next line contains n-integers which contain the value of this subset.</p>

<h3>Constraints</h3>
<p>T &lt;= 20</p>
<p>n &lt;= 50,000</p>
<p>Each element in the array &lt;= 1,000,000,000</p>

<h3>Output</h3>
<p>For each test case output the value of the maximum subset and the count of the subsets modulo 1000,000,009</p>
<p><strong>Example</strong></p>
<pre><strong>Input:</strong>
2
5
1 -1 1 -1 1
6
-200 -100 -100 -400 -232 -450

<strong>Output:</strong>
3 1
-100 2
</pre>