<p>You are given a tree (an acyclic undirected connected graph) with <strong>n</strong> nodes. The tree nodes are numbered from 1 to <strong>n</strong>. Each node has a color, white or black. All the nodes are black initially. We will ask you to perform some instructions of the following form:</p>
<ul>
<li><strong>0 u</strong>: ask for how many nodes are connected to <strong>u</strong>, two nodes are connected if all the node on the path from <strong>u</strong> to <strong>v</strong> (inclusive <strong>u</strong> and <strong>v</strong>) have the same color.</li>
<li><strong>1 u</strong>: toggle the color of <strong>u</strong> (that is, from black to white, or from white to black).</li>
</ul>
<h3>Input</h3>
<p>The first line contains a number <strong>n</strong> that denotes the number of nodes in the tree (1 ¡Ü <strong>n</strong> ¡Ü 10<sup>5</sup>). In each of the following <strong>n-1</strong> lines, there will be two numbers (<strong>u</strong>, <strong>v</strong>) that describes an edge of the tree (1 ¡Ü <strong>u</strong>, <strong>v</strong> ¡Ü <strong>n</strong>). The next line contains a number <strong>m</strong> denoting number of operations we are going to process (1 ¡Ü <strong>m</strong> ¡Ü 10<sup>5</sup>). Each of the following <strong>m</strong> lines describe an operation (<strong>t</strong>, <strong>u</strong>) as we mentioned above(0 ¡Ü <strong>t</strong> ¡Ü 1, 1 ¡Ü <strong>u</strong> ¡Ü <strong>n</strong>).</p>
<h3>Output</h3>
<p>For each query operation, output the corresponding result.</p>
<h3>Example</h3>
<pre style="text-align: left;"><strong>Input 1:</strong><br>5
1 2
1 3
1 4
1 5
3
0 1
1 1
0 1
<strong>Output 1:</strong><br>5
1</pre>
<pre style="text-align: left;"><strong><br>Input 2:<br></strong>7
1 2
1 3
2 4
2 5
3 6
3 7
4
0 1
1 1
0 2
0 3
<strong><br><br>Output 2:</strong><br>7
3
3<br><br><br><strong>Warning: large input/output data,be careful with certain languages</strong></pre>
<p>&nbsp;</p>
<p>&nbsp;</p>