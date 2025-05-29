<p>
Two players take part in the game <b>polygons</b>. A convex polygon with <i> n</i> vertices divided by
<i> n-3</i> diagonals into <i> n-2</i> triangles is necessary.
These diagonals may intersect in vertices of the polygon only. One of the triangles is black and the
remaining ones are white. Players proceed in alternate turns. Each player, when
its turn comes, cuts away one
triangle from the polygon. players are allowed to cut off triangles along the given
diagonals. The winner is the player who cuts away the black triangle.<br>
NOTE: We call a polygon <b> convex</b> if a segment joining any two points of
the polygon is contained in the polygon.
</p>

<h3>Task</h3>
<p>
Write a program which:&nbsp;
</p>
<ul>
 <li>reads from the standard input the description of the polygon,
 </li><li>verifies whether the player who starts the game has a winning strategy,
 </li><li>writes the result to the standard output. 
</li></ul>

<h3>Input</h3>
<p>
The number of test cases t is in the first line of input, then t test cases follow separated by an empty line.

The first line of each test case contains an integer <i>n</i>,<i> 4 &lt;= n &lt;=
50000</i>. This is the number of vertices in the polygon. The vertices of the polygon
are numbered, clockwise, from
<i> 0</i> to <i>n-1</i>.<br>
The next <i> n-2</i> lines comprise descriptions of triangles in the polygon. In the<i>
i+1</i>-th line, <i> 1 &lt;= i &lt;= n-2</i>, there are three non-negative
integers <i>a, b, c</i> 
separated by single spaces. Theses are numbers of vertices of the <i>i</i>-th triangle. The first triangle in a
sequence is black.
</p>

<h3>Output</h3>
<p>
The output for each test case should have one line with the word:
</p>
<ul>
 <li>YES, if the player, who starts the game has a winning
  strategy,</li>
 <li>NO, if he does not have a winning strategy.</li>
</ul>

<h3>Example</h3>
<pre><b>Sample input:</b>
1
6
0 1 2
2 4 3
4 2 0
0 5 4

<b>Sample output:</b>
YES</pre>

<b>Warning: large Input/Output data, be careful with certain languages</b>