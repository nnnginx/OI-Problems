<p>You are given&nbsp;an undirected graph with N verticies and M edges, where the weights are unique.&nbsp;</p>
<p>There is a function&nbsp;Cost(u, v), which is defined as follows:</p>
<p>While there is a path between vertex u and v, delete the edge with the smallest weight. Cost(u,v) is the sum of the weights of the edges that were deleted in this process.</p>
<p><img title="graph" src="../../content/francky:cost-graph" alt="graph" width="287" height="116"></p>
<p>For example, from the graph above (same as the sample input), Cost(2,6) is 2+3+4+5+6 = 20.</p>
<p>Given an undirected graph, your task is to calculate the sum of Cost(u,v) for all vertices u and v, where u &lt; v. Since the answer can get large, output the answer modulo 10^9.</p>

<h3>Input</h3>
<p>The first line of the input consists of two integers, N and M. (1 &lt;= N &lt;= 100,000, 0 &lt;= M &lt;= 100,000)</p>
<p>The next M lines consists of three integers, u, v, and w. This means that there is an edge between vertex u and v with weight w. (1 &lt;= u, v &lt;= N, 1 &lt;= w &lt;= 100,000)</p>

<h3>Output</h3>
<p>Output the sum specified in the problem statement.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
6 7<br>1 2 10<br>2 3 2<br>4 3 5<br>6 3 15<br>3 5 4<br>4 5 3<br>2 6 6<br><br>

<strong>Output:</strong>
256<br>
</pre>