<p>You must write a program that simulates placing spherical balloons into a rectangular box. 
</p><p>The simulation scenario is as follows. Imagine that you are given a rectangular box and a set of points. Each point represents a position where you might place a balloon. To place a balloon at a point, center it at the point and inflate the balloon until it touches a side of the box or a previously placed balloon. You may not use a point that is outside the box or inside a previously placed balloon. However, you may use the points in any order you like, and you need not use every point. Your objective is to place balloons in the box in an order that maximizes the total volume occupied by the balloons. 
</p><p>You are required to calculate the volume within the box that is not enclosed by the balloons. 
</p><h3>Input</h3>
<p>The input consists of several test cases. The first line of each test case contains a single integer n that indicates the number of points in the set (1&lt;=n&lt;=6). The second line contains three integers that represent the (x, y, z) integer coordinates of a corner of the box, and the third line contains the (x, y, z) integer coordinates of the opposite corner of the box. The next n lines of the test case contain three integers each, representing the (x, y, z) coordinates of the points in the set. The box has non-zero length in each dimension and its sides are parallel to the coordinate axes. 
</p><p>The input is terminated by the number zero on a line by itself. 
</p><h3>Output</h3>
<p>For each test case print one line of output consisting of the test case number followed by the volume of the box not occupied by balloons. Round the volume to the nearest integer. Follow the format in the sample output given below. 
</p><p>Place a blank line after the output of each test case.
</p><h3>Example</h3>
<pre><b>Input:</b>
2
0 0 0
10 10 10
3 3 3
7 7 7
0

<b>Output:</b>
Box 1: 774

</pre>