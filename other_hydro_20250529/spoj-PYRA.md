<p>Daniel is building towers. He has a big amount of block of the size 1x1xK (for any K). Out of them he is building towers according to the following rules: the longest block is put in the basement of the tower. Several towers built by the same rules can be put on this block. The distance between the bases of those towers should be 1 and the distance between the bases of the towers and the edges of the common basement should be 1. There should be a block of the length 1 on the top of each tower. Daniel encodes every tower with root tree. For example:

</p><div><img src="./24042/file/J17KYIeH.png"></div>
 
<p>The root of the tree corresponds to the basement of the tower. Its descendants correspond to the towers standing on it. The leaves correspond to the blocks of the size 1x1x1 on the tops. Given the root tree describing one of those structures, calculate the total volume of the structure.

</p><h3>Input</h3>
<p>The first line of input contains the number t - the number of tests. Next comes the description of t tests. Each test starts with an integer n - the number of nodes of the tree. This is followed by n-1 line, consisting of two integers a and b - number of nodes connected by an edge. Nodes are numbered from 0 to n-1. The root of the tree will always be a node with number 0. Otherwise the nodes and edges can go in any order.

</p><h3>Constraints</h3>
<p>1 &lt;= t &lt;= 25<br>
1 &lt;= n &lt;= 10^4

</p><h3>Output</h3>
<p>For each test case print the total volume of the structure build according to the rules in the problem statement.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
7
0 1
2 0
0 3
2 4
5 2
6 3
3
1 2
1 0

<b>Output:</b>
25
9

</pre>