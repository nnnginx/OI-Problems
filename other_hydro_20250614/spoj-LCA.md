<p style="text-align: justify;">A tree is an undirected graph in which any two vertices are connected by exactly one simple path. In other words, any connected graph without cycles is a tree. - Wikipedia&nbsp;</p>
<p style="text-align: justify;">The lowest common ancestor (LCA) is a concept in graph theory and computer science. Let T be a rooted tree with N nodes. The lowest common ancestor is defined between two nodes v and w as the lowest node in T that has both v and w as descendants (where we allow a node to be a descendant of itself). - Wikipedia</p>
<p style="text-align: justify;">Your task in this problem is to find the LCA of any two given nodes v and w in a given tree T.</p>
<h3 style="text-align: center;"><img src="./23140/file/z7AaMrAc.png" alt=""></h3>
<p><strong>For example the LCA of nodes 9 and 12 in this tree is the node number 3.</strong></p>
<h3 style="text-align: justify;">Input</h3>
<p style="text-align: justify;">The first line of input will be the number of test cases. Each test case will start with a number N the number of nodes in the tree, 1 &lt;= N &lt;= 1,000. Nodes are numbered from 1 to N. The next N lines each one will start with a number M the number of child nodes of the Nth node, 0 &lt;= M &lt;= 999 followed by M numbers the child nodes of the Nth node. The next line will be a number Q the number of queries you have to answer for the given tree T, 1 &lt;= Q &lt;= 1000. The next Q lines each one will have two number v and w in which you have to find the LCA of v and w in T, 1 &lt;= v, w &lt;= 1,000.</p>
<p style="text-align: justify;">Input will guarantee that there is only one root and no cycles.</p>
<h3 style="text-align: justify;">Output</h3>
<p style="text-align: justify;">For each test case print Q + 1 lines, The first line will have ¡°Case C:¡± without quotes where C is the case number starting with 1. The next Q lines should be the LCA of the given v and w respectively.</p>
<h3 style="text-align: justify;">Example</h3>
<pre><strong>Input:</strong>
1
7
3 2 3 4
0
3 5 6 7
0
0
0
0
2
5 7
2 7

<strong>Output:</strong>
Case 1:
3
1</pre>