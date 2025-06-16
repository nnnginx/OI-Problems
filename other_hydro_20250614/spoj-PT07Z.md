<p>
You are given an unweighted, undirected tree.
Write a program to output the length of the longest path (from one node to another) in that tree.
The length of a path in this case is number of edges we traverse from source to destination.
</p>

<h3>Input</h3>
<p>
The first line of the input file contains one integer <i>N</i> --- number of nodes in the tree
(0 &lt; <i>N</i> &lt;= 10000). Next <i>N</i>-1 lines contain <i>N</i>-1 edges of that tree --- Each line contains a pair (<i>u</i>, <i>v</i>) means
there is an edge between node <i>u</i> and node <i>v</i> (1 &lt;= <i>u</i>, <i>v</i> &lt;= <i>N</i>).
</p>

<h3>Output</h3>
<p>
Print the length of the longest path on one line.
</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
1 2
2 3

<b>Output:</b>
2
</pre>