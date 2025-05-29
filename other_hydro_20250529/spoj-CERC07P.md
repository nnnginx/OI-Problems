<p>In this problem, we will help the Faculty of Civil Engineering. They need a software to analyze
ground plans of buildings. Specifically, your task is to detect outlines of a building when all of
its corners are given.

</p><p></p><center><img src="/content/carl:cerc07p.jpg" alt="example"></center>

<p>You may assume that each building is a rectangular polygon with each of its sides being parallel
either with X or Y axis. Therefore, each of its vertex angles is exactly either 90 or 270 degrees.

</p><h3>Input</h3>
<p>The input contains several buildings. The description of each building starts with a single
positive integer N, the number of corners (polygon vertices), 1 &lt;= N &lt;= 1000. Then there are N
pairs of integer numbers X_i,Y_i giving coordinates of individual corners, |X_i|, |Y_i| &lt;= 10 000.

</p><p>You may assume that all corners are listed and no two of them have the same coordinates. The
polygon does always exist, it is closed, its sides do not intersect or touch (except neighboring
sides, of course), and it contains no "holes" inside. In other words, the outline is formed by one
closed line. The order of corners in the input file may be arbitrary.

</p><p>There is an empty line after each building, then the next one is described. After the last building,
there is a single zero that signals the end of input.

</p><h3>Output</h3>
<p>For each building, output one line containing N characters without any whitespace between
them. The characters should be uppercase letters that specify directions of individual walls
(sides) when the building outline is followed. "N" stands for North (the positive direction of the
Yaxis), "E" for East (the positive direction of the X axis), "W" for West, and "S" for South.
The "walk" should start in the vertex that has been given first in the input and always proceed
in the clockwise direction.

</p><h3>Example</h3>
<pre><b>Input</b>
4
0 0
2 2
0 2
2 0

6
1 1
2 2
0 1
1 0
0 2
2 0

0

<b>Output</b>
NESW
WNESWN
</pre>

<p><i>The second sample input corresponds to the picture.</i>
</p>