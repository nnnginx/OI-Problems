<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/ONBRIDGE/en/">English</a></td>
<td width="50%"><a href="/problems/ONBRIDGE/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Given a graph of N vertices, numbered from 0 to N - 1. Initially, there is no edge in the graph. Sequencially adding M undirected edges (u, v) to the graph (0 &lt;= u, v &lt;= N - 1). After adding an edge, you must print out the current number of bridges in the graph. The data guarantees that there is no request to add an existed edge, or an edge from a vertex to itself.</p>
<h3>Input</h3>
<p>The first line contains an integer T (T &lt;= 10) denotes the number of test cases. Each test case begins with 2 integers N (1 &lt;= N &lt;= 50000) and M (1 &lt;= M &lt;= 100000), followd by M lines, each line contains a pair of intergers (u, v) represents a request to add an edge (u, v) to the graph.</p>
<h3>Output</h3>
<p>After each request, print out the current number of bridges in the graph on a separate line.</p>
<h3>Example</h3>
<p>For the input data:</p>
<pre>1
5 10
3 0
0 2
1 0
1 3
1 4
2 4
4 0
2 1
2 3
3 4
</pre>
<p>the correct result is:</p>
<pre>1
2
3
1
2
0
0
0
0
0
</pre>
<p> </p>