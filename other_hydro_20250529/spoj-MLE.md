<p>Given <strong>n</strong> points on X-Y plane. To each point, you are to find the other point who is closest to it with respect to the Euclidean distance.</p>
<h3>Input</h3>
<p><strong>T</strong> (&lt;= 15) test cases. Each starts with an integer <strong>n</strong> (2&lt;= <strong>n</strong> &lt;=100000). Then <strong>n</strong> lines follow. Each contains two space-seperated integers, the X and Y coordinate of the corresponding point, respectively. No two points in one test case will coincide.</p>
<h3>Output</h3>
<p>For each test case, output <strong>n</strong> lines. The i-th of them should contain the squared distance between the i-th point from the input and its nearest neighbour.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
10
17 41
0 34
24 19
8 28
14 12
45 5
27 31
41 11
42 45
36 27
15
0 0
1 2
2 3
3 2
4 0
8 4
7 4
6 3
6 1
8 0
11 0
12 2
13 1
14 2
15 0

<strong>Output:</strong>
200
100
149
100
149
52
97
52
360
97
5
2
2
2
5
1
1
2
4
5
5
2
2
2
5
</pre>
<p><strong>Warning: enormous input/output data, be careful with certain languages</strong></p>