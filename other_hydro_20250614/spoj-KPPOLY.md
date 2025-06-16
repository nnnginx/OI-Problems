<p>You are given a convex polygon on Cartesian coordinate system. It has projections on X and Y-axis. You can arbitrary rotate this polygon. What minimum and maximum sum of projections can you achieve?

</p><h3>Input</h3>
<p>First line contains one integer number N (3 ¡Ü N ¡Ü 100) - number of polygon's vertices. Following N lines contain vertex coordinates X<sub>i</sub> and Y<sub>i</sub>. All numbers are integers. Vertices are given in clockwise or anticlockwise direction. No two vertices coincide. No three consecutive vertices lie on the same line. All coordinates do not exceed 10000 by absolute value.

</p><h3>Output</h3>
<p>Write minimum and maximum value of sum of the polygon's projections. Separate them by a space. Your answer should not differ with the correct one more than 10<sup>-6</sup>.

</p><h3>Example</h3>

<pre><b>Input:</b>
4
0 0
0 1
1 1
1 0

<b>Output:</b>
2 2.828427124
</pre>