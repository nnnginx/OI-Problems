<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/QTREE3/en/">English</a></td> 
<td width="50%"><a href="/problems/QTREE3/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>You are given a tree (an acyclic undirected connected graph) with N nodes. The tree nodes are numbered from 1 to N. In the start, the color of any node in the tree is white.
</p><p>We will ask you to perfrom some instructions of the following form:</p>
<ul>
<li><b>0 i</b> : change the color of the i-th node (from white to black, or from black to white);<br>
or
</li><li><b>1 v</b> : ask for the id of the first black node on the path from node 1 to node v. if it doesn't exist, you may return -1 as its result.
</li></ul>

<h3>Input</h3>
<p>In the first line there are two integers <b>N</b> and <b>Q</b>.
</p><p>In the next <b>N</b>-1 lines describe the edges in the tree: a line with two integers <b>a b</b> denotes an edge between <b>a</b> and <b>b</b>.
</p><p>The next <b>Q</b> lines contain instructions <b>"0 i"</b> or <b>"1 v"</b> (1 ¡Ü i, v ¡Ü N). </p>

<h3>Output</h3>
<p>For each "<b>1 v</b>" operation, write one integer representing its result.</p>

<h3>Example</h3>

<pre><b>Input:</b>
9 8
1 2
1 3
2 4
2 9
5 9
7 9
8 9
6 8
1 3
0 8
1 6
1 7
0 2
1 9
0 2
1 9 

<b>Output:</b>
-1
8
-1
2
-1
</pre>
<h3>Constraints &amp; Limits</h3>
<p>There are 12 real input files.
</p><p>For 1/3 of the test cases, N=5000, Q=400000.
</p><p>For 1/3 of the test cases, N=10000, Q=300000.
</p><p>For 1/3 of the test cases, N=100000, Q=100000.</p>