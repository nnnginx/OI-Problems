<p>You are given a tree (an acyclic undirected connected graph) with N nodes, and nodes numbered 1,2,3...,N. Each edge has an integer value assigned to it(note that the value can be negative). Each node has a color, white or black.
We define dist(a, b) as the sum of the value of the edges on the path from node a to node b.
</p>
<p>
All the nodes are white initially.
</p>
<p>
We will ask you to perfrom some instructions of the following form:
</p>

<ul>
<li><b>C a</b> : change the color of node a.(from black to white or from white to black)<br>
</li><li><b>A</b> : ask for the maximum dist(a, b), both of node a and node b must be white(a can be equal to b). Obviously, as long as there is a white node, the result will alway be non negative. 
</li></ul>

<h3>Input</h3>
<ul>
<li>In the first line there is an integer N (N &lt;= 100000)
</li><li>In the next N-1 lines, the i-th line describes the i-th edge: a line with three integers a b c denotes an edge between a, b of value c (-1000 &lt;= c &lt;= 1000)
</li><li>In the next line, there is an integer Q denotes the number of instructions (Q &lt;= 100000)
</li><li>In the next Q lines, each line contains an instruction "C a" or "A"
</li></ul>

<h3>Output</h3>
<p>For each "A" operation, write one integer representing its result.
If there is no white node in the tree, you should write "They have disappeared.".
</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
1 2 1
1 3 1
7
A
C 1
A
C 2
A
C 3
A

<b>Output:</b>
2
2
0
They have disappeared.

</pre>

<p>
<b>Some new test data cases were added on Apr.29.2008, all the solutions have been rejudged.</b>
</p>