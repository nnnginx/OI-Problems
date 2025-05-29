<p>&nbsp;</p>
<p>A graph initially consists of N  (1 ¡Ü N ¡Ü 100,000) unconnected vertices. The vertices are numbered from 1 to N.</p>
<p>Your task is to maintain that graph and answer connectivity queries.</p>
<p>All edges in the problem are <strong>undirected</strong>.</p>
<p>You will receive the following queries, where (1 ¡Ü A, B ¡Ü N) :</p>
<ul>
<li><strong>add</strong> A B : add an edge between  vertices  A and B, where initially there is no path between A and B.</li>
<li><strong>rem</strong> A B : remove edge between  vertices  A and B, where initially there is an edge between A and B.</li>
<li><strong>conn</strong> A B : print <strong>YES</strong> if there is a path between A and B and <strong>NO</strong> otherwise, where A and B are different.</li>
</ul>
<h3>Input</h3>
<p>The first line of input contains the number of vertices N and the number of queries M (1 ¡Ü M ¡Ü 100,000). The following M lines contain queries.</p>
<h3>Output</h3>
<p>For each <strong>conn</strong> query output <strong>YES</strong> or <strong>NO</strong>. Pay attention to letter case.</p>
<h3>Example</h3>
<pre><strong>Input:<br></strong>4 11<br>add 1 2<br>add 2 3<br>add 3 4<br>add 1 4<br>conn 4 2<br>rem 1 2<br>conn 2 4<br>rem 3 4<br>conn 4 2<br>add 2 4<br>conn 4 2<br><br><strong>Output:<br></strong>YES<br>YES<br>NO<br>YES<br><br>This example will be the first test case.</pre>