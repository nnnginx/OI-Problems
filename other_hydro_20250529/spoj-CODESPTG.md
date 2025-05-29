<p>&nbsp;</p>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">A clique in a graph is set of nodes such that there is an edge between any two distinct nodes in the set. It is well known that finding the largest clique in a graph is a computationally tough problem and no polynomial time algorithm is known for it. However, you wonder what is is the mininum size of the largest clique in any graph with N nodes and M edges. Of course, the graph should have at most one edge between any two nodes and no edges connecting a node to itself.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Input :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">The first line contains T the number of test cases. Each of the next T lines contain 2 integers : N, M</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Output T lines, one for each test case, containing the desired answer for the corresponding test case.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Input :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3 2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4 6</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">5 7</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Sample Output :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">4</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">3</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Constraints :</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= T &lt;= 100000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">2 &lt;= N &lt;= 10000</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">1 &lt;= M &lt;= N*(N-1)/2</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">Explanation:</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the second test case, the only valid graph having 4 nodes and 6 edges is one where each pair of nodes is connected. So the size of the largest clique cannot be smaller than 4.</div>
<div id="_mcePaste" style="position: absolute; left: -10000px; top: 0px; width: 1px; height: 1px; overflow-x: hidden; overflow-y: hidden;">For the third test case, it is easy to verify that any graph with 5 nodes and 7 edges will surely have a clique of size 3 or more.</div>
<p>&nbsp;</p>
<p>A clique in a graph is set of nodes such that there is an edge between any two distinct nodes in the set. It is well known that finding the largest clique in a graph is a computationally tough problem and no polynomial time algorithm is known for it. However, you wonder what is is the mininum size of the largest clique in any graph with N nodes and M edges. Of course, the graph should have at most one edge between any two nodes and no edges connecting a node to itself.</p>
<p>&nbsp;</p>
<p><strong>Input :</strong></p>
<p>The first line contains T the number of test cases. Each of the next T lines contain 2 integers : N, M</p>
<p>&nbsp;</p>
<p><strong>Output :</strong></p>
<p>Output T lines, one for each test case, containing the desired answer for the corresponding test case.</p>
<p>&nbsp;</p>
<p><strong>Sample Input :</strong></p>
<p>3</p>
<p>3 2</p>
<p>4 6</p>
<p>5 7</p>
<p>&nbsp;</p>
<p><strong>Sample Output :</strong></p>
<p>2</p>
<p>4</p>
<p>3</p>
<p>&nbsp;</p>
<p><strong>Constraints :</strong></p>
<p>1 &lt;= T &lt;= 100000</p>
<p>2 &lt;= N &lt;= 10000</p>
<p>1 &lt;= M &lt;= N*(N-1)/2</p>
<p>&nbsp;</p>
<p><strong>Explanation:</strong></p>
<p>For the second test case, the only valid graph having 4 nodes and 6 edges is one where each pair of nodes is connected. So the size of the largest clique cannot be smaller than 4.</p>
<p>For the third test case, it is easy to verify that any graph with 5 nodes and 7 edges will surely have a clique of size 3 or more.</p>
<p>&nbsp;</p>
<p>&nbsp;</p>