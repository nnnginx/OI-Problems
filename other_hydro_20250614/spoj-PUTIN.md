<h3>Input</h3>
<p>Multiple test cases, the number of them is given in the very first line.</p>
<p>For each test case:</p>
<p>The first line contains 3 space-separated integers K(2&lt;=K&lt;=30), S(2&lt;=S&lt;=10000), M(0&lt;=M&lt;=20). M lines follow, each contains K non-negative integers a<sub>ij</sub>(1&lt;=i&lt;=M, 1&lt;=j&lt;=K), which shows that there is one point (a<sub>i1</sub>, a<sub>i2</sub>, ... a<sub>ik</sub>) in the K-D hyperspace. No two point will be the same, and none of them lies on any (coordinate) axis.
</p><h3>Output</h3>
<p>For each test case:</p>
<p>Output a single integer which shows the number of the points B(b<sub>1</sub>, b<sub>2</sub>, ... b<sub>k</sub>) in the hyperspace satiesfied the following constraints:
</p><div align="justify">
<ul>
<li>
B is not on any (coordinate) axis.
</li><li>
For each 1&lt;= <i>i</i> &lt;= M, there exist <i>j</i>, 1&lt;=j&lt;=k, such that b<sub>j</sub> &lt; a<sub>ij</sub>.
</li><li>
For each 1&lt;=j&lt;=k, b<sub>j</sub> is a non-negative integer.
</li><li>
The sum of b<sub>j</sub> doesn't exceed S.
</li></ul>
</div>
<h3>Example</h3>
<pre><b>Input:</b>
1
2 4 2
1 3
2 1

<b>Output:</b>
2

<b>Hint</b>
<p>The two points are (1,1) and (1,2).
</p></pre>