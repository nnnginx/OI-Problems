<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MMINMAX/en/">English</a></td>
<td width="50%"><a href="/problems/MMINMAX/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p>
</p><p>&nbsp;</p><p>
Triangulation of surfaces has applications in the Finite Element Method of 
solid mechanics. The objective is to estimate the stress and strain on complex
objects by partitioning theminto small simple objects which are considered
incompressible. It is convenient to approximate a plane surface with a simple
polygon, i.e., a piecewise-linear, closed curve in the plane on m distinct
vertices, which does not intersect itself. A chord is a line segment between two
non-adjacent vertices of the polygon which lies entirely inside the polygon, 
so in particular, the endpoints of the chord are the only points of the chord 
that touch the  boundary of the polygon. 
</p><p>
A triangulation of the polygon, is any choice of m −3 chords, such 
that the polygon is divided into triangles. In a triangulation, 
o two of the chosen chords intersect each other, except at endpoints, 
and all of the remaining (unchosen) chords cross at least one of the
chosen chords. Fortunately, ﬁnding an arbitrary triangulation is a
fairly easy task, but what if you were asked to ﬁnd the best triangulation 
according to some measure?
</p>
<img src="../../../../../content/simes:MMINMAX.jpg" border="0">
<h3>Input</h3>
<p>&nbsp;</p><p>
On the first line of the input is a single positive integer n, telling
the number of test scenarios to follow. Each scenario begins with a line
containing one positive integer 2 &lt; m &lt; 50, being the number of vertices
of the simple polygon. The following m lines contain the vertices of the 
polygon in the order they appear along the border, going either clockwise
or counter clockwise, starting at an arbitrary vertex. 
</p><p>Each vertex is 
described by a pair of integers x y obeying 0 &lt;= x &lt;= 
10000 and 0 &lt;= y &lt;= 10 000.
</p><pre>SAMPLE INPUT
1
6
7 0
6 2
9 5
3 5
0 3
1 1
</pre>
<h3>Output</h3>
<p>&nbsp;</p>
<p>For each scenario, output one line containing the area of the largest triangle  in the triangulation of the polygon which has the smallest largest triangle. The area should be presented with one fractional decimal digit.</p>
<pre>SAMPLE OUTPUT
9.0
</pre>