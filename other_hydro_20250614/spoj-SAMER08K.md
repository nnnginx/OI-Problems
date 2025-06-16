<p>A polygon is said to be <em>inscribed</em> in a circle when all its vertices lie on that  circle.  In this problem you will be given a polygon inscribed in a circle, and you  must determine the minimum number of vertices that should be removed to  transform the given polygon into a <em>regular polygon</em>,  i.e., a polygon that is equiangular (all angles are  congruent) and equilateral (all edges have the same length).</p>
<p>When you remove a vertex <em>v</em> from a polygon you first remove  the vertex and the edges connecting it to its adjacent vertices <em>w</em><sub>1</sub> and   <em>w</em><sub>2</sub>, and then create a new edge connecting <em>w</em><sub>1</sub> and <em>w</em><sub>2</sub>.  Figure (a) below illustrates a polygon inscribed in a circle, with  ten vertices, and figure (b) shows a pentagon (regular polygon with  five edges) formed by removing five vertices from the polygon in (a). <br><br></p>
<img src="../../../content/disatoba:polygons.gif" border="0" alt="subir imagenes">
<p>&nbsp;</p>
<p>In this problem, we consider that any polygon must have at least three edges.</p>
<h3>Input</h3>
<p>The input contains several test cases. The first line of a test case  contains one integer <em>N</em> indicating the number of vertices of the  inscribed polygon (3   ¡Ü <em>N</em> ¡Ü 10<sup>4</sup>). The second line  contains <em>N</em> integers  <em>X</em><sub><em>i</em></sub> separated by single spaces (1   ¡Ü <em>X</em><sub><em>i</em></sub> ¡Ü 10<sup>3</sup>, for 0   ¡Ü <em>i</em> ¡Ü <em>N</em> -1).  Each <em>X</em><sub><em>i</em></sub> represents the length of the arc defined  in the inscribing circle, clockwise, by vertex <em>i</em> and vertex  (<em>i</em>+1)  mod <em>N</em>. Remember that  an <em>arc</em> is a segment of the circumference of a circle; do not  mistake it for a <em>chord</em>, which is a line segment whose  endpoints both lie on a circle.</p>
<p>The end of input is indicated by a line containing only one zero.</p>
<h3>Output</h3>
<p>For each test case in the input, your program must print a single  line, containing the minimum number of vertices that must be removed  from the given polygon to form a regular polygon. If it is not  possible to form a regular polygon, the line must contain only the  value <tt>-1</tt>.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
1000 1000 1000
6
1 2 3 1 2 3
3
1 1 2
10
10 40 20 30 30 10 10 50 24 26
0


<strong>Output:</strong>
0
2
-1
5

</pre>