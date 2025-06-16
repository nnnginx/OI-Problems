<p>

For products that are wrapped in small packings it is necessary that the sheet of paper containing the directions for use is folded until its size becomes small enough.
We assume that a sheet of paper is rectangular and only folded along lines parallel to its initially shorter edge.
The act of folding along such a line, however, can be performed in two directions: either the surface on the top of the sheet is brought together, or the surface on its bottom.
In both cases the two parts of the rectangle that are separated by the folding line are laid together neatly and we ignore any differences in thickness of the resulting folded sheet.

</p><p>

After several such folding steps have been performed we may unfold the sheet again and take a look at its longer edge holding the sheet so that it appears as a one-dimensional curve, actually a concatenation of line segments.
If we move along this curve in a fixed direction we can classify every place where the sheet was folded as either <code>type A</code> meaning a clockwise turn or <code>type V</code> meaning a counter-clockwise turn.
Given such a sequence of classifications, produce a drawing of the longer edge of the sheet assuming 90 degree turns at equidistant places.


</p><h3>Input Specification</h3><p>

The input contains several test cases, each on a separate line.
Each line contains a nonempty string of characters <tt>A</tt> and <tt>V</tt> describing the longer edge of the sheet.
You may assume that the length of the string is less than 200.
The input file terminates immediately after the last test case.

</p><h3>Output Specification</h3><p>

For each test case generate a PostScript drawing of the edge with commands placed on separate lines.
Start every drawing at the coordinates (300,420) with the command "<tt>300 420 moveto</tt>".
The first turn occurs at (310,420) using the command "<tt>310 420 lineto</tt>".
Continue with clockwise or counter-clockwise turns according to the input string, using a sequence of "<code>x</code> <code>y</code> <tt>lineto</tt>" commands with the appropriate coordinates.
The turning points are separated at a distance of 10 units.
Do not forget the end point of the edge and finish each test case by the commands <tt>stroke</tt> and <tt>showpage</tt>.


</p><p>

You may display such drawings with the <tt>gv</tt> PostScript interpreter, optionally after a conversion using the <tt>ps2ps</tt> utility.

</p><p>

</p><table cellpadding="0" cellspacing="0" width="100%"><tbody><tr>

<td valign="top">
<h3>Sample Input</h3><p>

</p><pre>V
AVV
</pre>

<h3>Sample Output</h3><p>

</p><pre>300 420 moveto
310 420 lineto
310 430 lineto
stroke
showpage
300 420 moveto
310 420 lineto
310 410 lineto
320 410 lineto
320 420 lineto
stroke
showpage
</pre>
</td>

<td valign="bottom">
<img src="./22280/file/Zkx1FB6h.png">
</td>

</tr></tbody></table>