<p align="justify">
There are many secret openings in the floor which are covered by a big heavy stone. When the stone is lifted up, a special mechanism detects this and activates poisoned arrows that are shot near the opening. The only possibility is to lift the stone very slowly and carefully. The ACM team must connect a rope to the stone and then lift it using a pulley. Moreover, the stone must be lifted all at once; no side can rise before another. So it is very important to find the centre of gravity and connect the rope
exactly to that point. The stone has a polygonal shape and its height is the same throughout the whole polygonal area. Your task is to find the centre of gravity for the given polygon.

</p><h3>Input</h3>
<p align="justify">The input consists of <var>T</var> test cases (equal to about 500). The number of them (<var>T</var>) is given on the first line of the input file.
Each test case begins with a line containing a single integer <var>N</var> (<var>3 &lt;= N &lt;= 1000000</var>) indicating the number of points that form the polygon. This is followed by <var>N</var> lines, each containing two integers <var>X<sub>i</sub></var> and <var>Y<sub>i</sub></var> (<var>|X<sub>i</sub>|, |Y<sub>i</sub>| &lt;= 20000</var>). These numbers are the coordinates of the <var>i</var>-th point. When we connect the points in the given order, we get a polygon. You may assume that the edges never touch each other (except the neighbouring ones) and that they never cross. The area of the polygon is never zero, i.e. it cannot collapse into a single line.

</p><h3>Output</h3>
<p align="justify">Print exactly one line for each test case. The line should contain exactly two numbers separated by one space. These numbers are the coordinates of the centre of gravity. Round the coordinates to the nearest number with exactly two digits after the decimal point (0.005 rounds up to 0.01). Note that the centre of gravity may be outside the polygon, if its shape is not convex. If there is such a case in the input data, print the centre anyway.

</p><h3>Example</h3>
<pre><b>Sample Input:</b>
2
4
5 0
0 5
-5 0
0 -5
4
1 1
11 1
11 11
1 11

<b>Sample output:</b>
0.00 0.00
6.00 6.00
</pre>