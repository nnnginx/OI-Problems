<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In the mathematical field of graph theory, a spanning tree T of a connected, undirected graph</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">G is a tree composed of all the vertices and some (or perhaps all) of the edges of G. Informally,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">a spanning tree of G is a selection of edges of G that form a tree spanning every vertex. That is,</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">every vertex lies in the tree, but no cycles (or loops) are formed. On the other hand, every</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">bridge of G must belong to T (a bridge is an edge whose deletion increases the number of</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">connected components).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">A spanning tree of a connected graph G can also be defined as a maximal set of edges of G that</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">contains no cycle, or as a minimal set of edges that connect all vertices. - Wikipedia</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">In graph theory, a cactus (sometimes called a cactus tree) is a connected graph in which any</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">two simple cycles have at most one vertex in common. Equivalently, every edge in such a graph</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">belongs to at most one simple cycle. Equivalently, every block (maximal subgraph without a</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">cut-vertex) is an edge or a cycle. - Wikipedia</div>
<p>In the mathematical field of graph theory, a spanning tree T of a connected, undirected graph G is a tree composed of all the vertices and some (or perhaps all) of the edges of G. Informally, a spanning tree of G is a selection of edges of G that form a tree spanning every vertex. That is, every vertex lies in the tree, but no cycles (or loops) are formed. On the other hand, every bridge of G must belong to T (a bridge is an edge whose deletion increases the number of connected components).</p>
<p>A spanning tree of a connected graph G can also be defined as a maximal set of edges of G that contains no cycle, or as a minimal set of edges that connect all vertices. - Wikipedia</p>
<p>In graph theory, a cactus (sometimes called a cactus tree) is a connected graph in which any two simple cycles have at most one vertex in common. Equivalently, every edge in such a graph belongs to at most one simple cycle. Equivalently, every block (maximal subgraph without a cut-vertex) is an edge or a cycle. - Wikipedia</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p><img style="vertical-align: middle; margin-left: 250px; margin-right: 250px;" src="file://tZ6LkPE0.png" alt="" width="234" height="351"></p>
<p style="text-align: center;"><span style="white-space: pre;"> </span><strong><span style="font-size: medium;">cactus graph</span></strong></p>
<p><span style="font-size: small;"><strong>&nbsp;</strong></span></p>
<p><strong>Your task in this problem is to count the number of ways you can convert a cactus graph to a&nbsp;</strong><span style="font-weight: bold;">spanning tree.</span></p>
<h3>Input</h3>
<p>&nbsp;</p>
<p>The first line of input will be the number of test cases. Each test case will start with a two numbers N and E where N is the number of vertices of the cactus graph, vertices are numbered from 1 to N, 3 &lt;= N &lt;= 81 and E is the number of edges in the graph, 2 &lt;= E &lt;= 120. The next E lines each one will have two numbers v and w and that means there is an edge between vertix v and w.</p>
<p>&nbsp;</p>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each test case print ��Case C: X�� without quotes where C is the case number starting with 1 and X is the number of ways you can convert the given cactus graph to a spanning tree.</p>
<p>&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 3
1 2
2 3
1 3
5 5
1 2
2 3
2 4
3 4
4 5

<strong>Output:</strong>
Case 1: 3
Case 2: 3</pre>