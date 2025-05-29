<p>A skating competition was organized on the largest icerink in
Byteland. The
icerink is a square of size 10000 * 10000. A competitor begins skating
at the START point chosen by referees and his task is to finish sliding
at the
FINISH point, also
chosen by referees. The points of START and FINISH are different. One
can slide in directions parallel to the sides of the
icerink. There are some obstacles placed on the icerink. Each obstacle
is a prism, which base is a polygon with sides parallel to the sides of
the
icerink. Each two adjacent sides of the base are always perpendicular.
The obstacles do not have
common points.
Each slide finishes up at the point where a competitor, for the first
time, meets the
wall of an obstacle, which is perpendicular to the direction of the
slide. In other words,
one can stop only when he crashes on a wall or in the FINISH point.
Falling out
of the icerink causes disqualification. Competitor may slide along
walls of
an obstacle.
</p>

<center>
<table width="442">
<tbody><tr><td width="486">
<img src="/content/piotrek:lodow1.gif" height="85" width="420">
</td></tr>
<tr><td width="486">
<img src="/content/piotrek:lodow2.gif" height="85" width="445">
</td></tr>
</tbody></table>
</center>

<p>
Decide, whether a competitor who slides according to the given rules may reach the finish
point, assuming he begun sliding from the starting point. If so, what is the minimal number
of slides he needs to do?
</p>

<h3>Task</h3> 

<p>
Write a program which:
</p><ul>
 <li>reads the description of the icerink, obstacles, and the coordinates of the
  start and finish point from the standard input,
 </li><li>verifies, whether a competitor who begins from the starting point and
  slides according the rules may reach the finish point, and if so, computes the minimal number
of slides he needs to do,
 </li><li>writes the result in the standard output.
</li></ul>  

<h3>Input</h3> 
<p>
The number of test cases t is in the first line of input, then t test cases follow separated by an empty line.
We define a system of coordinates to describe positions of objects
on a rink.
The rink is a square with vertices
(0,0),(10000,0),(10000,10000),(0,10000). In the first line of each test case 
there are two integers
<i>z<sub>1</sub> </i> and <i> z<sub>2</sub> </i> separated by a single space, 0&lt;=<i>z<sub>1</sub>,
z<sub>2</sub></i>&lt;=10000. The pair (<i>z<sub>1</sub>, z<sub>2</sub></i>) denotes coordinates of the START point. In the second line of the file there are two integers
<i>t<sub>1</sub> </i> and <i> t<sub>2</sub> </i> separated by single space, 0&lt;=<i>t<sub>1</sub>, t<sub>2</sub></i>&lt;=10000. The pair
(<i>t<sub>1</sub>, t<sub>2</sub></i>) denotes coordinates of the FINISH point. The third line of the file
contains one integer <i>s</i>, 1&lt;=<i>s</i>&lt;=2500. This is the number of obstacles. The following lines comprise descriptions
of <i> s </i> obstacles. Each description of an obstacle begins with the line
containing one
positive integer <i>r </i> equal to the number of walls (sides of the base)  of
the obstacle. In each of the following
<i> r</i> lines there are two integers<i> x</i> and <i> y</i>
separated by a single space. These are the coordinates of the vertices of the obstacle's base,
given in a clockwise order. (i.e. when going around the obstacle in this
direction the inside is on the left-hand side). The total number of side walls of
the obstacles does not exceed 10000.</p> 

<h3>Output</h3> 

<p> 

Your program should write for each test case:</p>
<ul>
<li>either one word 'NO' if it's impossible to get from the
  START point to the FINISH point
</li><li>or the minimal number of slides necessary to get to the FINISH point, if it
  is possible.
</li></ul>

<h3>Example</h3> 

<pre><b>Sample input:</b>
1
40 10
5 40
3
6
0 15
0 60
20 60
20 55
5 55
5 15
12
30 55
30 60
60 60
60 0
0 0
0 5
55 5
55 35
50 35
50 40
55 40
55 55
6
30 25
15 25
15 30
35 30
35 15
30 15

<b>Sample output:</b>
4
</pre>

<p>The sample input corresponds to the following situation:</p>
<p>
<img src="/content/piotrek:lodow3.gif" height="358" width="358">
</p><p>
These are the possible sequences of slides of length 4:
</p><p>
</p><table>
<tbody><tr>
<td><img src="/content/piotrek:lodow4.gif" height="152" width="152"></td>
<td><img src="/content/piotrek:lodow5.gif" height="152" width="152"></td>
<td><img src="/content/piotrek:lodow6.gif" height="152" width="152"></td>
</tr>
</tbody></table>

<b>Warning: large Input/Output data, be careful with certain languages</b>