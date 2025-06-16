<p>A discrete Voronoi diagram is a derivation of a Voronoi diagram. It is represented as a set of pixels. Each of the
generatrices lies on the center of some pixel. Each pixel belongs to the generatrix nearest from the center of the
pixel in the sense of Manhattan distance. The Manhattan distance d between two points (<i>x</i><sub>1</sub>, <i>y</i><sub>1</sub>) and (<i>x</i><sub>2</sub>, <i>y</i><sub>2</sub>) is
given by the following formula:
</p><center><i>d</i> = |<i>x</i><sub>1</sub> - <i>x</i><sub>2</sub>| + |<i>y</i><sub>1</sub> - <i>y</i><sub>2</sub>|</center>
<p>Your task is to find a set of generatrices which generates a given discrete Voronoi diagram. In the given diagram,
each generatrix is given a unique lowercase letter as its identifier, and each pixel is represented by the identifier
of the generatrix the pixel belongs to. If a pixel has multiple generatrices at the same distance from its center, it
belongs to the generatrix with the most preceding identifier among them (i.e. the smallest character code).

</p><h3>Input</h3>
<p>The input consists of multiple test cases.
</p><p>Each test case begins with a line containing two integers <i>W</i> (1 �� <i>W</i> �� 32) and <i>H</i> (1 �� <i>H</i> �� 32), which denote the
width and height of the discrete Voronoi diagram.
</p><p>The following <i>H</i> lines, each of which consists of <i>W</i> letters, give one discrete Voronoi diagram. Each letter
represents one pixel.
</p><p>The end of input is indicated by a line with two zeros. This is not a part of any test cases.

</p><h3>Output</h3>
<p>For each test case, print the case number and the coordinates of generatrices as shown in the sample output. Each
generatrix line should consist of its identifier, <i>x</i>-coordinate, and <i>y</i>-coordinate. Generatrices should be printed in
alphabetical order of the identifiers. Each coordinate is zero-based where (0, 0) indicates the center of the top-left
corner pixel of the diagram.
</p><p>You may assume that every test case has at least one solution. If there are multiple solutions, any one is acceptable.
</p><p>Print a blank line after every test case including the last one.

</p><h3>Example</h3>

<pre><b>Input:</b>
4 3
ooxx
ooxx
ooxx
4 1
null
4 4
aabb
aabb
ccdd
ccdd
0 0

<b>Output:</b>
Case 1:
o 0 0
x 2 0

Case 2:
l 2 0
n 0 0
u 1 0

Case 3:
a 0 0
b 2 0
c 0 2
d 2 2

</pre>