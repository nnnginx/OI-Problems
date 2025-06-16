<p>This is hard version of&nbsp;<a href="../DTPOLY/">DTPOLY</a>.</p>
<p>Determine the number of ways to cut a convex polygon with&nbsp;<strong>N</strong>&nbsp;vertices if the only cuts allowed are from vertex to vertex, each cut divides exactly one polygon into exactly two polygons, and you must end up with exactly&nbsp;<strong>K</strong>&nbsp;polygons. Consider each vertex distinct. For example, there are three ways to cut a square - the two diagonals and not cutting at all - but only two ways to cut it to form 2 polygons, and only one way to cut it to form 1 polygon. The order of cuts does not matter. Since the number of ways can be very large, you should return the number taken modulo <strong>M</strong>.</p>
<h3>Input</h3>
<p>Input contains&nbsp;several test cases, i-th line consists of 3&nbsp;integers:&nbsp;<strong>N<sub>i</sub></strong>&nbsp;(3 ¡Ü&nbsp;<strong>N<sub>i</sub></strong>, <strong>¦²</strong><strong>N<sub>i</sub></strong>&nbsp;¡Ü 10<sup>8</sup> over all test cases),</p>
<p><strong>K<sub>i</sub></strong>&nbsp;(1 ¡Ü&nbsp;<strong>K<sub>i&nbsp;</sub></strong>¡Ü&nbsp;<strong>N<sub>i&nbsp;</sub></strong>-&nbsp;2)&nbsp;and <strong>M<sub>i</sub>&nbsp;</strong>(1 &lt; <strong>M<sub>i</sub></strong> &lt; 2<sup>60</sup>), all pairs (<strong>N<sub>i</sub></strong>, <strong>K<sub>i</sub></strong>) are different.</p>
<h3>Output</h3>
<p>On the i-th line print the number of different ways to cut the polygon with <strong>N<sub>i</sub></strong>&nbsp;vertices into <strong>K<sub>i</sub></strong> pieces modulo <strong>M<sub>i</sub></strong>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
4 2 100
6 3 100
10000000 2 1000000007
10000000 5000000 1000000014000000049</pre>
<pre><strong>Output:</strong>
2
21
984650007
780127215155143528
</pre>