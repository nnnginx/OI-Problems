<p style="text-align: justify;">An air combat is on the way, you are asked to command this war. Now planes of enemy are full of the sky. A plane is described with three-dimensional coordinate (x, y, z)(1000&lt;x, y, z&lt;1200), and all coordinates are integers. As is show below:</p>
<p style="text-align: center;"><img style="vertical-align: middle;" title="Example " src="../../content/fameoflight:1.jpg" alt="" width="422" height="279"></p>
<p style="text-align: justify;">You have created a missile which can destroy all the planes in a cube whose center is (x, y, z), and the cube can be as large as (x-r, y-r, z-r) (x+r, y+r, z+r). This missile is so fierce that it will destroy not only enemy in that space, but also friends. And after that a position is occupied by a plane belongs to the opposite side before the explosion, that is to say an enemy plane will be replaced by a friend, a friend will be replaced by an enemy.</p>
<p style="text-align: justify;">You want to reduce our loss, so you need to know which side a plane belongs to in a position.</p>
<p><img src="file:///C:/DOCUME%7E1/ADMINI%7E1/LOCALS%7E1/Temp/moz-screenshot.png" alt=""></p>
<p>&nbsp;</p>
<h3>Input</h3>
<p>The first line contains the number of scenarios. <br> For each scenario you are given a line containing x1 y1 z1 x2 y2 z2, defining the two corners A(x1, y1, z1), B(x2, y2, z2) (1000&lt;= x1&lt;x2, y1&lt;y2, z1&lt;z2 &lt;=1200) of the sky. The combat is so fierce that every point in the cube is occupied by an enemy plane at first.</p>
<p>Next line is a number of operation q.</p>
<p>Next q lines: (0&lt;q&lt;10000)</p>
<p>A character ¡®U¡¯:&nbsp; followed by 4 integers, a center point M(xi, yi, zi) ,the range is ri.</p>
<p>A character ¡®Q¡¯:&nbsp; followed by 3 integers, a position N(xi, yi, zi), if a plane belongs to us, print ¡±Friend¡± else print ¡±Enemy¡±.</p>
<p>Points M and N are all in cube given above.</p>
<h3>Output</h3>
<p>Print a line for every ¡®Q¡¯ operation.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br><p>1</p><p>1000 1000 1000 1002 1002 1002</p><p>4</p><p>U 1000 1000 1000 0</p><p>U 1001 1001 1001 1</p><p>Q 1000 1000 1000</p><p>Q 1001 1001 1001</p><strong>Output:</strong><br><p>Enemy</p><p>Friend</p></pre>