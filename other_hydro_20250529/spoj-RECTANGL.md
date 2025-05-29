<p>You are given a set <i>S</i> of <i>N</i> points in the plane and must count the number of distinct axis-parallel rectangles whose four vertices all lie in <i>S</i> (that is, count those rectangles which have two sides parallel to the <b>x</b>-axis, and the other two sides parallel to the <b>y</b>-axis).

</p><h3>Input</h3>
<p>The first line of the input is <i>N</i> (1 ¡Ü <i>N</i> ¡Ü 250000), the number of points in <i>S</i>.  <i>N</i> lines then follow, where the <b>i</b>-th line is of the form "<i>x<sub>i</sub></i> <i>y<sub>i</sub></i>", giving the coordinates of a point (<i>x<sub>i</sub></i>, <i>y<sub>i</sub></i>) in <i>S</i>.  All given points are distinct, and all coordinates fit into a 32-bit signed integer.

</p><h3>Output</h3>
<p> Your output should consist of a single number, the number of distinct axis-parallel rectangles whose four vertices all lie in <i>S</i>, followed by a newline.

</p><h3>Example</h3>

<pre><b>Input:</b>
6
-1 0
-1 1
0 0
0 1
1 0
1 1

<b>Output:</b>
3
</pre>