<p><em>"In graph theory, an arborescence is a directed graph in which, for a vertex v called the root and any other vertex u, there is exactly one directed path from v to u. In other words, an arborescence is a directed, rooted tree in which all edges point away from the root. Every arborescence is a directed acyclic graph."</em></p>
<p>-- from Wikipedia, the free encyclopedia</p>
<p>You are given a directed graph with <em>N</em> vertices, and your task is to count the number of different arborescences of size <em>N</em> that can be found in the given graph.</p>
<p>Two arborescences are considered different when they consist of different edges.</p>
<h3>Input</h3>
<p>Input consists of multiple test cases.</p>
<p>For each test case, the first line contains one integer <em>N</em> described as above.</p>
<p>N lines follows, each consists of <em>N</em> characters, either '0' or '1', representing the adjacency matrix of the graph.</p>
<p>The directed graph contains edge (<em>i</em>,<em>j</em>) if and only if the <em>j</em>th character of the <em>i</em>th line of the matrix is '1'.</p>
<p>The graph consists of no more than 8 vertices.</p>
<p>End of input is indicated by a line consisting of a single 0.</p>
<h3>Output</h3>
<p>For each test case, output one line consisting of one single integer, the number of arborescences.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
00
00
2
01
10
0

<strong>Output:</strong>
0
2
</pre>