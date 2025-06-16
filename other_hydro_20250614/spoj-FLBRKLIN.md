<p align="justify">We have a cartesian coordinate system drawn on a sheet of paper. Let us consider broken lines that can be drawn with a single pencil stroke from the left to the right side of the sheet. We also require that for each segment of the line the angle between the straight line containing this segment and the OX axis belongs to [-45бу, 45бу] range. A broken line fulfilling above conditions is called a flat broken line. Suppose we are given <i>n</i> distinct points with integer coordinates. What is the minimal number of flat broken lines that should be drawn in order to cover all the points (a point is covered by a line if it belongs to this line)? </p>

<h3>Example</h3>
<p align="center"><img src="/content/ahven:lam.gif"></p>
<p align="justify">For 6 points whose coordinates are (1,6), (10,8), (1,5), (2,20), (4,4), (6,2) the minimal number of flat broken lines covering them is 3. </p>

<h3>Task</h3>
<p align="justify">Write a program that for each test case:</p>
<div align="justify">
<ul align="justify">
        <li align="justify">reads the number of points and their coordinates; </li>
        <li align="justify">computes the minimal number of flat broken lines that should be drawn to cover all the points; </li>
        <li align="justify">outputs the result.</li>
</ul>
</div>

<h3>Input</h3>
<p align="justify">The number of test cases <i>t</i> is in the first line of input, then <i>t</i> test cases follow separated by an empty line.</p>
<p align="justify">In the first line of a test case there is one positive integer <i>n</i>, not greater than 30000, which denotes the number of points. In the following <i>n</i> lines there are coordinates of points. Each line contains two integers <i>x</i>, <i>y</i> separated by a single space, 0  &lt;=  <i>x</i>  &lt;=  30000, 0  &lt;=  <i>y</i>  &lt;=  30000. The numbers in the <i>i</i>-th line are the coordinates of the <i>i</i>-th point. </p>

<h3>Output</h3>
<p align="justify">For each test case you should output one line with the minimal number of flat broken lines that should be drawn to cover all the points.</p>

<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
6
1 6
10 8
1 5
2 20
4 4
6 2

<b><tt>Sample output:</tt></b>
3
</pre>