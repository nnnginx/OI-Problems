<p>Using a sheet of paper and scissors, you can cut out two faces to
form a cylinder in the following way: </p>
<ol>
<li>Cut the paper horizontally (parallel
to the shorter side) to get two rectangular parts.</li>
<li>From the first part, cut out a circle
of maximum radius. The circle will form the bottom of the cylinder.</li>
<li>Roll the second part up in such a way
that it has a perimeter of equal length with the circle's
circumference, and attach one end of the roll to the circle.
Note that the roll may have some overlapping parts in order
to get the required length of the perimeter.</li>
</ol>
<p>Given the dimensions of the sheet of paper, can you calculate the
biggest possible volume of a cylinder which can be constructed using the
procedure described above? </p>

<h4>Input Specification</h4>
<p>
The input consists of several test cases.
Each test case consists of two numbers <strong>w</strong> and
<strong>h</strong> (<i>1 �� w �� h �� 100</i>), which indicate
the width and height of the sheet of paper.
</p>
<p>The last test case is followed by a line containing two zeros.
</p>
<h4>Output Specification</h4>
<p>
For each test case, print one line with the biggest possible volume
of the cylinder. Round this number to 3 places after the decimal point.
</p>
<h4>Sample Input</h4>
<pre>10 10
10 50
10 30
0 0
</pre>
<h4>Sample Output</h4>
<pre>54.247
785.398
412.095
</pre>
<hr>
<i>In the first case, the optimal cylinder has a radius of about
1.591549,
in the second case, the optimal cylinder has a radius of 5,
and in the third case, the optimal cylinder has a radius of
about 3.621795.</i>