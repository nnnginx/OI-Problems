<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">We define a Beta graph as a set of nodes connected by edges such that one node is connected to another node by at most one edge and no node has an edge starting and ending on itself. Each node has a finite number called 'degree' asssociated with it which is the number of edges connecting that node to the rest of the nodes.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">There are n nodes in a given Beta graph.Those nodes with degree=0 are removed from the graph.Then those, who had degree=1 were removed(and so are the edges connecting that node to the rest of the nodes). Then those, who had degree equal to 2,3,...,n-1 were removed(including their edges).</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow: hidden;">For any Beta graph with n nodes find the maximum number of nodes that can remain after the above procedure is completed.</div>
<p>We define a Beta graph as a set of nodes connected by edges such that one node is connected to another node by at most one edge and no node has an edge starting and ending on itself. Each node has a finite number called 'degree' asssociated with it which is the number of edges connecting that node to the rest of the nodes.</p>
<p>There are n nodes in a given Beta graph.Those nodes with degree=0 are removed from the graph.Then those, who had degree=1 were removed(and so are the edges connecting that node to the rest of the nodes). Then those, who had degree equal to 2,3,...,n-1 were removed(including their edges).</p>
<p>For any Beta graph with n nodes find the maximum number of nodes that can remain after the above procedure is completed.</p>
<p>&nbsp;</p>
<h3>Input</h3>
<p><span style="color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12.800000190734863px; line-height: 13.600000381469727px;">The first input line contains one number t ¡ª amount of tests (1¡Üt¡Ü10^5). Each of the following t lines contains one integer number n (0¡Ün¡Ü10^5).</span></p>
<h3>Output</h3>
<p><span style="color: #333333; font-family: 'lucida grande', tahoma, verdana, arial, sans-serif; font-size: 12.800000190734863px; line-height: 13.600000381469727px;">For each test case output in a separate line the maximum number of nodes that can remain after the above procedure is completed.</span>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
1</pre>
<pre>3

<strong>Output:</strong>
1</pre>