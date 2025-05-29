<p>A rooted tree is being built. Initially, there is only one node in the tree, having number 1 and value 0. You are to perform Q (Q&lt;=200000) queries, each of them is one of the following two types:</p>
<ul>
<li>1 X Y - Add a new vertex to the tree with parent X (It's guaranteed that node X is already in the tree)&nbsp;and value Y (1&lt;=Y&lt;=10^9). Its number will be the smallest positive integer that is not a number of a node yet. For example, the first query of this type will add a vertex with number 2, then 3, then 4 and so on.</li>
<li>2 X - Consider the children of node X. For each of them, let's sum up the values of all nodes in their subtrees. You are asked to print the maximum of those sums.</li>
</ul>
<h3>Input</h3>
<p>The first line contains an integer Q - the number of queries. Each of the next Q lines contains one of the queries.</p>
<h3>Output</h3>
<p>Print the answers for all queries of the second type, one answer per line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7<br>1 1 3<br>2 1<br>2 2<br>1 2 5<br>2 1<br>1 1 4<br>2 1</pre>
<pre><strong>Output:</strong>
3<br>0<br>8<br>8</pre>