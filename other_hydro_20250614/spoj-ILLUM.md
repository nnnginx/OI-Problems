<p>Two cubes and a light bulb are placed in a three-dimensional euclidean space. You are expected to find out
if one of them casts shadow on the other one and if so, calculate the area of this shadow.</p>
<h3>Input</h3>
<p>Multiple test cases. For each test case: </p>
<p>The first line of the input contains the coordinates of the bulb. It is followed
by two groups of four lines each that describe the cubes. Each line of the
cube description contains the coordinates of a vertex (see the figure where
the vertices are marked and labeled in the same order as they are given in the
input).</p>
<p><img src="./22893/file/CM5AEqX5.png"></p>
<p>All the coordinates are given with 5 digits after decimal point. It is guaranteed that the cubes do not intersect,
the light bulb is outside both of them, and doesn¡¯t lie on any of the planes that contain their faces. A light
bulb should be regarded as a point light source.</p>
<p>Input terminates by EOF.</p>
<h3>Output</h3>
<p>For each test case: </p>
<p>The output should contain a single line with two numbers separated with a space character. The first one is
the number of the cube that has a shadow on it (1 or 2). The second is the area of the shadow. If none of the given cubes casts shadow on the other the output should contain a single number -1.</p>
<p><b>Note:</b> if your output has an error with absolute value less than 10<sup>-2</sup>, it will be judged as Accepted. i.e. You may output any number of digits after decimal point.</p>
<h3>Example</h3>
<pre><b>Input:</b>
-1.00000 1.00000 1.00000
0.00000 0.00000 0.00000
2.00000 0.00000 0.00000
0.00000 2.00000 0.00000
0.00000 0.00000 2.00000
5.00000 0.00000 0.00000
7.00000 0.00000 0.00000
5.00000 2.00000 0.00000
5.00000 0.00000 2.00000
0.00000 0.00000 0.00000
1.00000 1.00000 1.00000
2.00000 1.00000 1.00000
1.00000 2.00000 1.00000
1.00000 1.00000 2.00000
-1.00000 -1.00000 -1.00000
-1.00000 -2.00000 -1.00000
-2.00000 -1.00000 -1.00000
-1.00000 -1.00000 -2.00000

<b>Output:</b>
2 4.000
-1
</pre>