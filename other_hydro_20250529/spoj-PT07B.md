<p>You are given an unweighted, undirected tree <i>T</i>.
We say <i>T</i> is special iff it has this property: </p>

<p>"All nodes of degree greater than or equal to 3 are surrounded by at most two nodes of degree two or greater."</p>

<p>Finding maximal size subtree of this tree so that it's a special tree. </p>

<h3>Input</h3>
<p>The first line of the input file contains one integer <i>N</i> --- number of nodes in the tree
(0 &lt; <i>N</i> &lt;= 10<sup>6</sup>). Next <i>N</i>-1 lines contain <i>N</i>-1 edges of that tree --- Each line contains a pair (<i>u</i>, <i>v</i>) means
there is an edge between node <i>u</i> and node <i>v</i> (1 &lt;= <i>u</i>, <i>v</i> &lt;= <i>N</i>).
</p>

<h3>Output</h3>
<p>At the first line, output number of nodes in the optimal subtree you found.
Next lines, print all edges belong to that subtree, each line contains a pair <i>u</i> <i>v</i> means an edge between node <i>u</i> and node <i>v</i>.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
5
1 2
2 3
2 4
2 5

<b>Output:</b>
5
1 2
2 3
2 4
2 5
</pre>