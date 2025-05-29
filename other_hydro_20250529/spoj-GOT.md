<p>
There's a tree, with each vertex assigned a number. For each query (a, b, c), you are asked whether there is a vertex on the path from a to b, which is assigned number c?
</p>

<h3>Input</h3>
<p>There are multiple cases, end by EOF.</p>

<p>For each case, the first line contains n (n &lt;= 100000) and m (m &lt;= 200000), representing the number of vertexes (numbered from 1 to n) and the number of queries.</p>

<p>Then n integers follows, representing the number assigned to the i-th vertex.</p>

<p>Then n-1 lines, each of which contains a edge of the tree.</p>

<p>Then m lines, each of which contains three integers a, b and c (0 &lt;= c &lt;= n), representing a query.</p>

<h3>Output</h3>
<p>You should output "<code>Find</code>" or "<code>NotFind</code>"&nbsp;for every query on one line.</p>

<p>Output a blank line AFTER every case.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
5 5
1 2 3 4 5
1 2
1 3
3 4
3 5
2 3 4
2 4 3
2 4 5
4 5 1
4 5 3

<strong>Output:</strong>
NotFind
Find
NotFind
NotFind
Find</pre>