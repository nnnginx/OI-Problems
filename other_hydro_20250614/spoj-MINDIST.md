<p>Given an weighted tree, you are to find two nodes A and B of the tree(A and B needn't to be different), such that the length of the path between A and B is less than or equals to a given integer S, and the maximum distance from each node of the tree to this path is minimum.</p>
<h3>Input</h3>
<p>The first line of the input contains a single integer T, the number of test cases. T blocks follow.</p>
<p>For each test case, the first line contains two space-separated integer N (1&lt;=N&lt;=100000) and S(0&lt;=S&lt;=100000000).N-1 lines follow, each contains three integers X(1&lt;=X&lt;=N), Y(1&lt;=Y&lt;=N) and Z(1&lt;=Z&lt;=1000), denotes that there is an (undirected) edge weighted Z between node X and Y. The input is correct.</p>
<h3>Output</h3>
<p>T lines, each contains a single integer denoted the minimum distance.</p>
<h3>Example</h3>
<pre><b>Input:</b>
2
5 2
1 2 5
2 3 2
2 4 4
2 5 3
8 6
1 3 2
2 3 2
3 4 6
4 5 3
4 6 4
4 7 2
7 8 3

<b>Output:</b>
5
5

</pre>
<b>Warning: large input/output data, be careful with certain languages</b>