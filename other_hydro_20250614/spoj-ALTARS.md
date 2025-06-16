<p>
According to Chinese folk beliefs evil spirits can move only on a
straight line. It is of a great importance when temples are built. The
temples are constructed on rectangular planes with sides parallel to
the
north - south or east - west directions.
No two of the rectangles have common points. An entrance is situated in
the middle of one of four walls and its width is equal to the half of
the
length of the wall. An altar appears in the center of the temple, where
diagonals of the rectangle intersect. If an evil spirit appears in this
point, a temple will be profaned. It may happen only if there exists a
ray which runs from an altar, through an entrance to infinity and
neither intersects nor touches walls of any temple (on a plane parallel
to the plane of a construction area),
i.e. one can draw at a construction area a line which starts at the
altar and
runs to the infinity without touching any wall.&nbsp;
</p>

<h3>Task</h3>
<p>
Write a program which:&nbsp;
</p><ul>

<li>reads descriptions of the temples from the standard input,

</li><li>verifies which temples could be profaned,

</li><li>writes their numbers to the standard output.
</li></ul>

<h3>Input</h3>

<p>
The number of test cases t is in the first line of input, then t test cases follow separated by an empty line.
In the first line of each test case one integer <i>n</i>, the number of temples
<i> 1 &lt;= n &lt;= 1000,</i> is written.
</p>

<p>
In each of the following <i> n</i> lines there is a description of one temple (in <i>i</i>-th line a description
of the<i> i-</i>th
temple). The description of a temple consists of four non-negative
integers,
not greater than 8000 and a letter E, W, S or N. Two first numbers are
coordinates of a temple's northern-west corner and two following are
coordinates of an opposite southern-east corner. In order to
specify coordinates of a point first we give its geographical
longitude, which increases from the
west to the east, and then its latitude, which increases from the south
to the
north. The fifth element of the description indicates the wall with the
entrance (E - Eastern, W - Western, S - Southern, N - Northern).
The
elements of the temple's description are separated by single spaces.
</p>

<h3>Output</h3>

<p>In the following lines of the output for each test case your program should
write in ascending order numbers of the temples, which may
be profaned by an evil spirit. Each number is placed in a separate
line. If there are no such numbers, you should
write one word:
NONE.&nbsp;
</p>

<h3>Example</h3>
<p>
<tt>Sample input</tt>
</p><pre>6
1 7 4 1 E
3 9 11 8 S
6 7 10 4 N
8 3 10 1 N
11 4 13 1 E
14 8 20 7 W
</pre>
<tt>Sample output</tt>
<pre>1
2
5
6
</pre>
<p>
The picture shows the temples described in the example. The dashed lines show possible routes of evil spirits.<br>
<img src="/content/piotrek:oltarze.gif" height="274" width="621">
</p>