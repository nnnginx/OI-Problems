<p>Determine the number of ways to cut a convex polygon with <strong>N</strong> sides if the only cuts allowed are from vertex to vertex, each cut divides exactly one polygon into exactly two polygons, and you must end up with exactly <strong>K</strong> polygons. Consider each vertex distinct. For example, there are three ways to cut a square - the two diagonals and not cutting at all - but only two ways to cut it to form 2 polygons, and only one way to cut it to form 1 polygon. The order of cuts does not matter. Since the number of ways is very large, you should return the number taken modulo 1000000000 (one billion). If there is no way to cut the polygon into <strong>K</strong> pieces, return -1.&nbsp;&nbsp;&nbsp;&nbsp;</p>
<h3>Input</h3>
<ul>
<li>Input contains only 2 integers in one line:&nbsp;<strong>N</strong> (1 ¡Ü N ¡Ü 100) and <strong>K</strong> (1 ¡Ü K ¡Ü 100).</li>
</ul>
<h3>Output</h3>
<ul>
<li>Output contains only one integer, the number of different ways to cut the polygon into K pieces.</li>
</ul>
<h3>Example</h3>
<pre><strong>Input:</strong><br>4 2<br><br><strong>Output:</strong><br>2<br></pre>