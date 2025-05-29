<p>	You are given a node-labeled rooted tree with <i>n</i> nodes.
</p>
<p>
	Define the query (<i>x</i>, <i>k</i>): Find the node whose label is <i>k</i>-th largest in the subtree of the node <i>x</i>.
	Assume no two nodes have the same labels.</p>

<h3>Input</h3>
<p>
The first line contains one integer <i>n</i> (1 &lt;= <i>n</i> &lt;= 10<sup>5</sup>).
The next line contains <i>n</i> integers <i>l<sub>i</sub></i> (0 &lt;= <i>l<sub>i</sub></i> &lt;= 10<sup>9</sup>) which denotes the label of the <i>i</i>-th node.
</p>

<p>
Each line of the following <i>n</i> - 1 lines contains two integers <i>u</i>, <i>v</i>.
They denote there is an edge between node <i>u</i> and node <i>v</i>.
Node 1 is the root of the tree.
</p>
<p>
The next line contains one integer <i>m</i> (1 &lt;= <i>m</i> &lt;= 10<sup>4</sup>) which denotes the number of the queries.
Each line of the next <i>m</i> contains two integers <i>x</i>, <i>k</i>. (<i>k</i> &lt;= the total node number in the subtree of <i>x</i>)
</p>
<h3>Output</h3>
<p>For each query (<i>x</i>, <i>k</i>), output the index of the node whose label is the <i>k</i>-th largest in the subtree of the node <i>x</i>.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
5
1 3 5 2 7
1 2
2 3
1 4
3 5
4
2 3
4 1
3 2
3 2

<b>Output:</b>
5
4
5
5
</pre>