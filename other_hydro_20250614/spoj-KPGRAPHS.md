<p>In this problem your task is to count the amount of graphs of different types. We only consider undirected graphs without self-loops. Every pair of vectices can be connected with at most one edge. Graphs are labeled, i.e. if a graph has N vertices, then each of them has a unique label from 1 to N.</p>
<p>We will be interested in three types of graphs - connected, eulerian and bipartite. A graph is connected, if and only if there is at least one path between any pair of vertices. A graph is eulerian, if and only if it's connected and there is a cycle that goes through every edge exactly once. A graph is bipartite, if and only if we can split all of its vertices into two subsets A and B, such that every edge has one endpoint in A and another in B.</p>
<h3>Input</h3>
<p>The first line of the input contains one integer number T (1 &lt;= T &lt;= 1000) - the number of test cases.</p>
<p>Next T lines contain different test cases. Each test case contains one integer number N (1 &lt;= N &lt;= 1000) - the number of vertices in a graph.</p>
<h3>Output</h3>
<p>For each test case, output the number of connected graphs, the number of euleran graphs and the number of bipartite graphs - all modulo 1000000007. See examples for the required format. Output one additional empty line after each test case.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2<br>1<br>2<br><br><strong>Output:</strong><br>Connected: 1<br>Eulerian: 1<br>Bipartite: 1<br><br>Connected: 1<br>Eulerian: 0<br>Bipartite: 2<br><br></pre>