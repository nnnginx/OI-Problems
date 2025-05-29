<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MTREECOL/en/">English</a></td>
<td width="50%"><a href="/problems/MTREECOL/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>Bob is very interested in the data structure of a tree. A tree is a directed graph in which a special node is singled out, called the "root" of the tree, and there is a unique path from the root to each of the other nodes. <br> <br>Bob intends to color all the nodes of a tree with a pen. A tree has  N nodes, these nodes are numbered 1, 2, ..., N. Suppose coloring a node takes 1 unit of time, and after finishing coloring one node, he is allowed to color another. Additionally, he is allowed to color a node only when its father node has been colored. Obviously, Bob is only allowed to color the root in the first try. <br> <br>Each node has a ��coloring cost factor��, Ci. The coloring cost of each node depends both on Ci and the time at which Bob finishes the coloring of this node. At the beginning, the time is set to 0. If the finishing time of coloring node i is Fi, then the coloring cost of node i is Ci * Fi. <br> <br>For example, a tree with five nodes is shown in Figure-1. The coloring cost factors of each node are 1, 2, 1, 2 and 4. Bob can color the tree in the&nbsp; order 1, 3, 5, 2, 4, with the minimum total coloring cost of 33.</p>
<p><a href="http://tinypic.com" target="_blank"></a></p>
<p style="text-align: center;"><img src="../../../../../../content/simes:MTREECOL.jpg" border="0" height="400"></p>
<p>Given a tree and the coloring cost factor of each node, please help Bob to find the minimum possible total coloring cost for coloring all the nodes.</p>
<h3>Input</h3>
<p>The input consists of several test cases. The first line of each case contains two integers N and R (1 &lt;= N &lt;= 1000, 1 &lt;= R &lt;= N), where N is the number of nodes in the tree and R is the node number of the root node. The second line contains N integers, the i-th of which is Ci (1 &lt;= Ci &lt;= 500), the coloring cost factor of node  i. Each of the next N-1lines contains two space-separated node numbers V1 and V2, which are the endpoints of an edge in the tree, denoting that V1 is the father node of V2.</p>
<p>No edge will be listed twice, and all edges will be listed.</p>
<p>A test case of N = 0 and R = 0 indicates the end of input, and should not be processed.</p>
<pre><br>Sample Input<br>5 1 <br>1 2 1 2 4 <br>1 2 <br>1 3 <br>2 4 <br>3 5 <br>0 0 </pre>
<h3>Output</h3>
<p>For each test case, output a line containing the minimum total coloring cost required for Bob to color all the nodes</p>
<pre><br>Sample output<br>33</pre>
<p> </p>