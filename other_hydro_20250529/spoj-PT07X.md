<p>
You are given an unweighted, undirected tree.
Write a program to find a vertex set of minimum size in this tree such that each edge has as least one of its end-points in that set.
</p>

<h3>Input</h3>
<p>
The first line of the input file contains one integer <i>N</i> --- number of nodes in the tree
(0 &lt; <i>N</i> &lt;= 100000). Next <i>N</i>-1 lines contain <i>N</i>-1 edges of that tree --- Each line contains a pair (<i>u</i>, <i>v</i>) means
there is an edge between node <i>u</i> and node <i>v</i> (1 &lt;= <i>u</i>,<i>v</i> &lt;= <i>N</i>).
</p>

<h3>Output</h3>
<p>
Print number of nodes in the satisfied vertex set on one line.
</p>

<h3>Example 1</h3>

<pre><b>Input:</b>
3
1 2
1 3

<b>Output:</b>
1

<b>Explanation:</b>
The set can be {1}
</pre>


<h3>Example 2</h3>

<pre><b>Input:</b>
3
1 2
2 3

<b>Output:</b>
1

<b>Explanation:</b>
The set can be {2}
</pre>