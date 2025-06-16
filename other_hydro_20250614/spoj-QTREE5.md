<p>You are given a tree (an acyclic undirected connected graph) with N nodes. The tree nodes are numbered from 1 to N. We define dist(a, b) as the number of edges on the path from node a to node b.
</p>
<p>Each node has a color, white or black. All the nodes are black initially.
</p>
<p>We will ask you to perfrom some instructions of the following form:
</p>

<ul>
<li>0 i : change the color of i-th node(from black to white, or from white to black).
</li><li>1 <b>v</b> : ask for the minimum dist(u, <b>v</b>), node u must be white(u can be equal to <b>v</b>). Obviously, as long as node <b>v</b> is white, the result will always be 0. 
</li></ul>


<h3>Input</h3>
<ul>
<li>In the first line there is an integer N (N &lt;= 100000)
</li><li>In the next N-1 lines, the i-th line describes the i-th edge: a line with two integers a b denotes an edge between a and b.
</li><li>In the next line, there is an integer Q denotes the number of instructions (Q &lt;= 100000)
</li><li>In the next Q lines, each line contains an instruction "0 i" or "1 <b>v</b>"
</li></ul>


<h3>Output</h3>
<p>For each "1 <b>v</b>" operation, print one integer representing its result.
If there is no white node in the tree, you should write "<b>-1</b>".
</p>



<h3>Example</h3>

<pre><b>Input:</b>
10
1 2
1 3
2 4
1 5
1 6
4 7
7 8
5 9
1 10
10
0 6
0 6
0 6
1 3
0 1
0 1
1 3
1 10
1 4
1 6

<b>Output:</b>
2
2
2
3
0

</pre>