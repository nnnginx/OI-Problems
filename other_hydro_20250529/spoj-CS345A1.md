<p>There are n vertical line segments colored red and there are n horizontal line segments colored blue.<br>We wish to find the number of red-blue pairs of intersecting segments.</p>
<p><img title="Red Blue segments in a unit square" src="../../../../../../content/simes:CS345A1.png" alt="Red Blue segments in a unit square"></p>
<p>These line segments are inside a unit square. Each blue segment is created by generating 3 random numbers (x_1, x_2, y) in the interval [0, 1]. These 3 numbers represent the segment joining (x_1, y) and (x_2, y). Red segments are generated similarly.</p>
<h3>Input</h3>
<p>First line contains the number of segments n (n &lt;= 100000)</p>
<p>next n lines define the blue segments. Each line contains 3 floating point numbers (in [0, 1]) x_1 x_2 y representing the segment joining (x_1, y) and (x_2, y).</p>
<p>next n lines define the red segments. Each line contains 3 floating point numbers (in [0, 1]) y_1 y_2 x representing the segment joining (x, y_1) and (x, y_2).</p>
<h3>Output</h3>
<p>Print a single line containing the number of intersections.</p>
<p><em>Note: Toucing line segments also count as intersecting. For ex - blue segment joining (0.1, 0.2) and (0.3, 0.2) intersects with red segment joining (0.3, 0.4) and (0.3, 0.2).</em></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3<br>0.36295 0.557494 0.184032<br>0.0479258 0.214097 0.508344<br>0.234284 0.969098 0.739363<br>0.499323 0.739797 0.138495<br>0.829265 0.22551 0.290582<br>0.791082 0.069214 0.450979

<strong>Output:</strong>
4<br><strong></strong></pre>