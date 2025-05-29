<p>Given a graph with N (2 ¡Ü N ¡Ü 5,000) vertices numbered 1 to N and M (1 ¡Ü M ¡Ü 30,000) undirected, weighted edges, compute the <a href="http://en.wikipedia.org/wiki/Maximum_flow_problem">maximum flow / minimum cut</a> from vertex 1 to vertex N.</p>

<h3>Input</h3>
<p>The first line contains the two integers N and M. The next M lines each contain three integers A, B, and C, denoting that there is an edge of capacity C (1 ¡Ü C ¡Ü 10<sup>9</sup>) between nodes A and B (1 ¡Ü A, B ¡Ü N). Note that it is possible for there to be duplicate edges, as well as an edge from a node to itself.</p>

<h3>Output</h3>
<p>Print a single integer (which may not fit into a 32-bit integer) denoting the maximum flow / minimum cut between 1 and N.</p>

<h3>Example</h3>

<pre><b>Input:</b>
4 6
1 2 3
2 3 4
3 1 2
2 2 5
3 4 3
4 3 3

<b>Output:</b>
5
</pre>

<p>Viewing the problem as max-flow, we may send 3 units of flow through the path 1 - 2 - 3 - 4 and 2 units of flow through the path 1 - 3 - 4. Viewing the problem as min-cut, we may cut the first and third edges. Either way the total is 5.</p>

<p>Note: see also <a href="http://www.spoj.com/problems/MATCHING/">http://www.spoj.com/problems/MATCHING/</a>.</p>