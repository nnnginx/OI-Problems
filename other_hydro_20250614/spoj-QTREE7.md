<p>You are given a tree (an acyclic undirected connected graph) with n nodes. The tree nodes are numbered from 1 to <strong>n</strong>. Each node has a color, white or black, and a weight. We will ask you to perfrom some instructions of the following form:</p>
<ul>
<li><strong>0 u</strong>: ask for the maximum weight among the nodes which are connected to <strong>u</strong>, two nodes are connected if all the node on the path from <strong>u</strong> to <strong>v</strong> (inclusive <strong>u</strong> and <strong>v</strong>) have a same color.</li>
<li><strong>1 u</strong>: toggle the color of <strong>u</strong>(that is, from black to white, or from white to black).</li>
<li><strong>2 u w</strong>: change the weight of <strong>u</strong> to <strong>w</strong>.</li>
</ul>
<h3>Input</h3>
<p>The first line contains a number <strong>n</strong> denoted how many nodes in the tree(1 ¡Ü <strong>n</strong> ¡Ü 10<sup>5</sup>). The next <strong>n</strong>-1 lines, each line has two numbers (<strong>u</strong>, <strong>v</strong>) describe a edge of the tree(1 ¡Ü <strong>u</strong>, <strong>v</strong> ¡Ü n).  The next 2 lines, each line contains <strong>n</strong> number, the first line is the initial color of each node(0 or 1), and the second line is the initial weight, let's say Wi, of each node(|<strong>Wi</strong>| ¡Ü 10<sup>9</sup>).  The next line contains a number <strong>m</strong> denoted how many operations we are going to process(1 ¡Ü <strong>m</strong> ¡Ü 10<sup>5</sup>). The next <strong>m</strong> lines, each line describe a operation (<strong>t</strong>, <strong>u</strong>) as we mentioned above(0 ¡Ü <strong>t</strong> ¡Ü 2, 1 ¡Ü <strong>u</strong> ¡Ü <strong>n</strong>, |<strong>w</strong>| ¡Ü 10<sup>9</sup>).</p>
<h3>Output</h3>
<p>For each query operation, output the corresponding result.</p>
<h3>Example</h3>
<pre style="text-align: left;"><strong>Input 1:</strong><br><div id="_mcePaste" style="position: absolute; left: -10000px; top: 300px; width: 1px; height: 1px; overflow: hidden;">5</div>5
1 2
1 3
1 4
1 5
0 1 1 1 1
1 2 3 4 5
3
0 1
1 1
0 1
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 300px; width: 1px; height: 1px; overflow: hidden;">1 2</div><br><strong>Output 1:</strong><br>1
5</pre>
<pre style="text-align: left;"><strong><br>Input 2:<br></strong>7
1 2
1 3
2 4
2 5
3 6
3 7
0 0 0 0 0 0 0
1 2 3 4 5 6 7
4
0 1
1 1
0 2
0 3<strong><br><br>Output 2:</strong><br>7
5
7<br><br><br><strong>Warning: large input/output data,be careful with certain languages</strong></pre>
<p>&nbsp;</p>
<p>&nbsp;</p>