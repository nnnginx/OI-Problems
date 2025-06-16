<p>
Bruce Force is standing in the forest.  He wonders what is the tree trunk the farthest
away which is not blocked from his view by other tree trunks.
</p>
<p>
Bruce has made a map of the trees in the forest.
The map shows his current position as the origin of a cartesian coordinate system.
Tree <i>i</i> is shown on the map as a circle with the center (<i>x<sub>i</sub>, y<sub>i</sub></i>) and radius <i>r<sub>i</sub></i>.
You may assume that a tree trunk is visible if and only if there exists a line segment on
the map from the origin (0,0) to a point on the border of the circle representing the tree trunk, where the line segment
does not intersect or touch another circle.
</p>

<h3>Input</h3>
<p>The input contains several test cases.
The first line of each test case contains one number <i>n</i> (<i>1 ¡Ü n ¡Ü 1000</i>),
where <i>n</i> specifies how many trees are on the map.
The following <i>n</i> lines contain 3 integers <i>x<sub>i</sub></i>, <i>y<sub>i</sub></i>, <i>r<sub>i</sub></i> each,
(<i>-10000 ¡Ü x<sub>i</sub>, y<sub>i</sub> ¡Ü 10000 </i>, <i>1 ¡Ü r<sub>i</sub> ¡Ü 1000 </i>)
where (<i>x<sub>i</sub></i>, <i>y<sub>i</sub></i>) is the center of the circle representing tree trunk <i>i</i>,
and <i>r<sub>i</sub></i> is the radius of the circle.
You may assume that no two circles in the input intersect, i.e., for
any two circles, the distance between their centers is more than the sum of their radii.
Moreover, you may assume that no circle contains the origin.

</p>
<p>
The last test case is followed by a line containing one zero.
</p>

<h3>Output</h3>
<p>For each test case, print one line with the maximum euclidean distance from
the origin to a visible tree. The distance to a tree should be measured
using the point of the tree closest to the origin, no matter if this point is
in fact visible or not.
</p>
<p>
Round the answer to 3 digits after the decimal point.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
10 10 11
1 1 1
-20 -10 20
5
1 2 2
-2 1 1
2 -1 1
-1 -2 2
10000 -10000 1000
0
<b>Output:</b>
3.142
1.236
</pre>