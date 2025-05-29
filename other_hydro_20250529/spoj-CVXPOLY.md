<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/CVXPOLY/en/">English</a></td> 
<td width="50%"><a href="/problems/CVXPOLY/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>You are given n points in the 2-D cartesian coordinate system. You are to determine the number of convex polygons with 3 or more vertices which can be formed by choosing a subset of the given points. To make matters simple, the input obeys the following conditions: </p>
<ul>
<p>(1) No 3 points in the input are collinear. </p>
<p>(2) No 2 points will have the same coordinates. </p>
</ul>
<p>Since the result can be quite large, you are required to output ( result % 1234567 ) instead. </p>

<h3>Input</h3>
<p>First line contains an integer T, the number of test cases. In each test case, first line contains n, the number of points in the corresponding test case, next n lines contain 2 space separated integers denoting the coordinate of ith point. Absolute value of the coordinates do not exceed 10000. </p>

<h3>Output</h3>
<p>T lines each corresponding to the answer of corresponding test case. </p>

<h3>Example</h3>

<pre><b>Input:</b>
2
4
0 0
2 0
2 2
0 2
6
0 0
2 0
2 2
0 2
1 -1
1 3

<b>Output:</b>
5
42
</pre>
<h3>Constraints</h3>
<pre>Input Set 1 : numberOfTestCases &lt;= 100, 3 &lt;= n &lt;= 10 timeLimit: 5 seconds 
Input Set 2 : numberOfTestCases &lt;= 50, 3 &lt;= n &lt;= 100 timeLimit: 5 seconds 
</pre>