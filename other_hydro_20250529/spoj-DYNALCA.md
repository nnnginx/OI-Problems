<p>&nbsp;</p>
<p>A forest of rooted trees initially consists of N  (1 ¡Ü N ¡Ü 100,000) single-vertex trees. The vertices are numbered from 1 to N.</p>
<p>You must process the following queries, where (1 ¡Ü A, B ¡Ü N) :</p>
<ul>
<li><strong>link</strong> A B : add an edge from  vertex  A to B, making A a child of B, where initially A is a root vertex, A and B are in different trees.</li>
<li><strong>cut</strong> A : remove edge from A to its parent, where initially A is a non-root vertex.</li>
<li><strong>lca</strong> A B : print the lowest common ancestor of A and B, where A and B are in the same tree.</li>
</ul>
<h3>Input</h3>
<p>The first line of input contains the number of initial single-vertex trees N and the number of queries M (1 ¡Ü M ¡Ü 100,000). The following M lines contain queries.</p>
<h3>Output</h3>
<p>For each <strong>lca</strong> query output the lowest common ancestor (vertex number between 1 and N).</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>5 9<br>lca 1 1<br>link 1 2<br>link 3 2<br>link 4 3<br>lca 1 4<br>lca 3 4<br>cut 4<br>link 5 3<br>lca 1 5<br><br><strong>Output:<br></strong>1<br>2<br>3<br>2<br><br></pre>