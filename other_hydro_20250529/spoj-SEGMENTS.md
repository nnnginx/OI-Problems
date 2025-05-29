<p>There are N horizontal line segments in the plane.  The ith segment
has some height h<sub>i</sub> (which may be negative) and runs from x = a<sub>i</sub>
to x = b<sub>i</sub> (a<sub>i</sub> &lt; b<sub>i</sub>).  Segments do not contain their endpoints.
You must draw a set of vertical lines (note <i>lines</i> and not <i>line segments</i>) so that every given horizontal segment is
intersected at least once and at most R times by vertical lines in such a way that R
is minimized.

</p><h3>Input</h3>
<p>The first line of the input is N (1 ¡Ü N ¡Ü 400), the number of
horizontal line segments.  N lines then follow, where the ith line
is "a<sub>i</sub> b<sub>i</sub> h<sub>i</sub>".  Each of a<sub>i</sub>,b<sub>i</sub>,h<sub>i</sub> are 32-bit signed
integers.  Horizontal segments may overlap.

</p><h3>Output</h3>
<p>Your output should consist of a single integer, the smallest value of
R that is achievable, followed by a newline.

</p><h3>Example</h3>

<pre><b>Input:</b>
3
0 1 5
0 2 -2
1 2 7

<b>Output:</b>
2
</pre>