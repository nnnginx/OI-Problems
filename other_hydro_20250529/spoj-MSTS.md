<p>Your task is simple in this problem: count the number of <b>minimum spanning tree</b> (<a href="http://en.wikipedia.org/wiki/Minimum_spanning_tree">Wikipedia</a>) in a simple undirected graph. The number of minimum spanning trees mean in how many ways you can select a subset of the edges of the graphs which forms a minimum spanning tree.

</p><h3>Input</h3>
<p>The first line of input contains two integers <b>N</b> (1 ¡Ü <b>N</b> ¡Ü 100), <b>M</b> (1 ¡Ü <b>M</b> ¡Ü 1000). Nodes are labeled from 1 to <b>N</b>. In the following <b>M</b> lines, every line contains three integers <b>a<sub>i</sub></b>, <b>b<sub>i</sub></b>, <b>c<sub>i</sub></b>, representing an undirected edge from node <b>a<sub>i</sub></b> to node <b>b<sub>i</sub></b>, with weight <b>c<sub>i</sub></b>. (1 ¡Ü <b>a<sub>i</sub></b> ¡Ù <b>b<sub>i</sub></b> ¡Ü <b>N</b>, 1 ¡Ü <b>c<sub>i</sub></b> ¡Ü 1,000,000,000). You can assume there is at most one edge between two nodes, and the graph described by input is connected. 

</p><h3>Output</h3>
<p>Print the <b>answer</b> % 31011. 

</p><h3>Example</h3>

<pre><b>Input:</b>
4 6
1 2 1
1 3 1
1 4 1
2 3 2
2 4 1
3 4 1

<b>Output:</b>
8
</pre>