<p>
Technicians in a pathology lab analyze digitized images of slides.
Objects on a slide are selected for analysis by a mouse click on the object.
The perimeter of the boundary of an object is one useful measure.
Your task is to determine this perimeter for selected objects.
</p>
<p>
The digitized slides will be represented by a rectangular grid of periods,
'<tt>.</tt>', indicating empty space, and the capital letter '<tt>X</tt>', indicating part
of an object.  Simple examples are
</p>
<p>
<b><tt>XX   Grid 1       .XXX  

Grid 2</tt></b>
<br><b><tt>XX               
.XXX</tt></b>
<br><b><tt>                 
.XXX</tt></b>
<br><b><tt>                 
...X</tt></b>
<br><b><tt>                 
..X.</tt></b>
<br><b><tt>                 
X...</tt></b>

</p>
<p>
An <tt>X</tt> in a grid square indicates that the entire grid
square, including its boundaries, lies in some object.  The <tt>X</tt>
in the center of the grid below is <i>adjacent</i> to the <tt>X</tt> in any
of the 8
positions around it. The grid squares for any two adjacent <tt>X</tt>'s
overlap on an edge or corner, so they are connected.

</p>

<p>
<tt>XXX</tt>
<br><tt>X<b>X</b>X   </tt> Central <tt>X</tt> and adjacent <tt>X</tt>'s
<br><tt>XXX</tt>

</p>

<p>
An object consists of the grid squares of all <tt>X</tt>'s that
can be linked to one another through a sequence of adjacent <tt>X</tt>'s. 
In Grid 1, the whole grid is filled by one object.  In Grid 2 there
are two objects.  One object contains only the lower left grid square. 
The remaining <tt>X</tt>'s belong to the other object.

</p>

<p>
The technician will always click on an <tt>X</tt>, selecting the object containing
that <tt>X</tt>.  The coordinates of the click are recorded.  Rows and
columns are numbered starting from 1 in the upper left hand corner. 
The technician could select the object in Grid 1 by clicking on row 2 and
column 2.  The larger object in Grid 2 could be selected by clicking
on row 2, column 3. The click could not be on row 4, column 3.
</p>

<p>
<img src="./22896/file/47XynMSo.png" hspace="20" height="105" width="54" align="LEFT"> One
useful statistic is the perimeter of the object.  Assume each <tt>X</tt> corresponds
to a square one unit on each side.  Hence the object in Grid 1 has
perimeter 8 (2 on each of four sides).  The perimeter for the
larger object in Grid 2 is illustrated in the figure at
the left.  The length is 18.
</p>

<p>
Objects will not contain any totally enclosed holes, so the leftmost
grid patterns shown below could <i>NOT</i> appear.
The variations on the right could appear:
</p><p><b><tt>Impossible   Possible</tt></b><b><tt></tt></b>
</p><p><b><tt>XXXX         XXXX  
XXXX   XXXX</tt></b>

<br><b><tt>X..X         XXXX  
X...   X...</tt></b>
<br><b><tt>XX.X         XXXX  
XX.X   XX.X</tt></b>
<br><b><tt>XXXX         XXXX  

XXXX   XX.X</tt></b><b><tt></tt></b>
</p><p><b><tt>.....        .....  ..... 
.....</tt></b>
<br><b><tt>..X..        ..X.. 
..X..  ..X..</tt></b>

<br><b><tt>.X.X.        .XXX. 
.X...  .....</tt></b>
<br><b><tt>..X..        ..X.. 
..X..  ..X..</tt></b>
<br><b><tt>.....        ..... 

.....  .....</tt></b><b></b>
</p>

<p>
The input will contain one or more grids.  Each grid is preceded
by a line containing the number of rows and columns in the grid and the
row and column of the mouse click.  All numbers are in the range 1-20. 
The rows of the grid follow, starting on the next line, consisting of '<tt>.</tt>'
and '<tt>X</tt>' characters.

</p>

<p>
The end of the input is indicated by a line containing four zeros. 
The numbers on any one line are separated by blanks.  The grid rows
contain no blanks.
</p>

<p>
For each grid in the input, the output contains a single line
with the perimeter of the specified object.
</p>

<pre><b>Input:</b>
2 2 2 2
XX
XX
6 4 2 3
.XXX
.XXX
.XXX
...X
..X.
X...
5 6 1 3
.XXXX.
X....X
..XX.X
.X...X
..XXX.
7 7 2 6
XXXXXXX
XX...XX
X..X..X
X..X...
X..X..X
X.....X
XXXXXXX
7 7 4 4
XXXXXXX
XX...XX
X..X..X
X..X...
X..X..X
X.....X
XXXXXXX
0 0 0 0
</pre>

<pre><b>Output:</b>
8
18
40
48
8
</pre>