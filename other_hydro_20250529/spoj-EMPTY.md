<p>
We call a cuboid <b> regular</b>  if:
</p>
<ul>
 <li>one of its vertices is a point with coordinates (0,0,0),
 </li><li>edges beginning in this vertex lie on the positive semi-axes of the coordinate
  system,
 </li><li>the edges are not longer than 10<sup>6</sup>
</li></ul>
<p>
There is given a set <b> A</b> of points of space, whose coordinates are integers
from the interval
[1..10<sup>6</sup>]. We try to find a regular cuboid of maximal volume which does not
contain any of the points from the set <b>A</b>. A point belongs to the cuboid
if it belongs to the interior of the
cuboid, i.e. it is a point of the cuboid, but not of its wall.
</p>

<h3>Task</h3>
<p>Write a program which:</p>
<ul>
 <li>reads from the standard input the coordinates of points from the set <b>A</b>,
 </li><li>finds one of the regular cuboids of maximal volume which does not contain any points from the set
  <b>A</b>,
 </li><li>writes the result to standard output.
</li></ul>

<h3>Input</h3>
<p>Input begins with a line containing integer t&lt;=10, the number of test cases. t test cases follow.
</p><p>In the first line of each test case one non-negative integer <i>n</i> is written
(<i> n</i> &lt;= <i>5000</i>). It is the number of elements in the set
<b>A</b>. In the following
<i> n</i> lines of the input there are triples of integers from the interval
[1..10<sup>6</sup>], which are the X, Y and Z coordinates of points from <b>A</b>, repectively. Numbers in each line are separated by single spaces.
</p>

<h3>Output</h3>
<p>
For each test case there should be three integers separated by single
spaces. These are the X, Y and Z coordinates (respectively) of the vertex of the
regular cuboid of maximal volume. If there is more than one such a cuboid, choose whichever. We require that all coordinates be positive.
</p>

<h3>Example</h3>
<pre><b>Sample input:</b>
1
4
3 3 300000
2 200000 5
90000 3 2000
2 2 1000

<b>Sample output:</b>
1000000 200000 1000
</pre>