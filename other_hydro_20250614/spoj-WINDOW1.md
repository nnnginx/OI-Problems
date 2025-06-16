<p align="justify">We have a polygon chosen in the cartesian coordinate system. Sides of the polygon are parallel to the axes of coordinates. Every two consecutive sides are perpendicular and coordinates of every vertex are integers. We have also given a window that is a rectangle whose sides are parallel to the axes of coordinates. The interior of the polygon (but not its periphery) is coloured red. What is the number of separate red fragments of the polygon that can be seen through the window?</p>

<h3>Example</h3>
<p align="justify">Look at the figure below: </p>
<p align="center"><img src="/content/ahven:okno.gif"></p>
<p align="justify">There are two separate fragments of the polygon that can be seen through the window. </p>

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads descriptions of a window and a polygon; </li>
        <li align="justify">computes the number of separate red fragments of the polygon that can be seen through the window; </li>
        <li align="justify">outputs the result.</li>
</ul></div>

<h3>Input</h3>
<p align="justify">The number of test cases <i>t</i> is in the first line of input, then <i>t</i> test cases follow separated by an empty line.</p>
<p align="justify">In the first line of a test case there are four integers <i>x</i><sub>1</sub>, <i>y</i><sub>1</sub>, <i>x</i><sub>2</sub>, <i>y</i><sub>2</sub> from the range [0..10000], separated by single spaces. The numbers <i>x</i><sub>1</sub>, <i>y</i><sub>1</sub> are the coordinates of the top-left corner of the window. The numbers <i>x</i><sub>2</sub>, <i>y</i><sub>2</sub> are the coordinates of the bottom-right corner of the window. The next line of the input file contains one integer <i>n</i>, 4 &lt;= <i>n</i> &lt;= 5000, which equals the number of vertices of the polygon. In the following <i>n</i> lines there are coordinates of polygon's vertices given in anticlockwise direction, i.e. the interior of the polygon is on the left side of its periphery when we move along the sides of the polygon according to the given order. Each line contains two integers <i>x</i>, <i>y</i> separated by a single space, 0 &lt;= <i>x</i> &lt;= 10000, 0 &lt;= <i>y</i> &lt;= 10000. The numbers in the <i>i</i>-th line, are coordinates of the <i>i</i>-th vertex of the polygon. </p>

<h3>Output</h3>
<p align="justify">For each test case you should output one line with the number of separate red fragments of the polygon that can be seen through the window.</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
0 5 8 1
24
0 0
4 0
4 2
5 2
5 0
7 0
7 3
3 3
3 2
2 2
2 4
1 4
1 5
2 5
2 6
3 6
3 5
4 5
4 6
5 6
5 4
7 4
7 7
0 7

<b><tt>Sample output:</tt></b>
2
</pre>