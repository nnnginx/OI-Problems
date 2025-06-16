<p>
A large cube (of size NxNxN) is given. At the beginning it consists of small blocks (1x1x1) and each block is painted in some color (different blocks may have the same color). But in the process of exploitation some blocks have disappeared. Given 6 photos of the unstable cube you have to calculate the maximum possible number of blocks that still remain in the unstable cube. It is possible that the unstable 
cube consists of more than one part.
</p>

<h3>Input</h3>
<p><i>t</i> ¨C the number of test cases, then <i>t</i> test cases follow. <br>
<i>N</i> - size of the big cube <i>[1 &lt;= N &lt;= 10]</i><br>
In the next <i>N</i> lines views of the cube from 6 sides are described (in the following order: from the front, left, back, right, from above, from below). Each such view is represented by a table of size <i>NxN</i> in which different letters denote different colors, and the symbol "." (point) means that it is possible to see all the way through the cube at this point. Consecutive views are separated by exactly one space.</p>
<p>
The bottom border of the top view corresponds to the top border of the front view, and the top border of the bottom view - to the bottom border of the front view. For the front, back, left and right views the top and bottom sides of a view correspond to the top and bottom of the cube. 
</p>
<p>
The input file is correct, i.e. each test case describes a possible configuration.
</p>

<h3>Output</h3>
<p>For each test case output one integer: the required maximum number of blocks remaining in the unstable cube.<br>

</p><h3>Example</h3>
<p>
</p><pre><b>Input:</b>
2
3
.R. YYR .Y. RYY .Y. .R.
GRB YGR BYG RBY GYB GRB
.R. YRR .Y. RRY .R. .Y.
2
ZZ ZZ ZZ ZZ ZZ ZZ
ZZ ZZ ZZ ZZ ZZ ZZ

<b>Output:</b>
11
8
</pre>