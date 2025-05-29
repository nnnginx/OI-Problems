<p>Ant Smart is on a surface of cylinder now. He wants to move to another position of the cylinder¡¯s surface. Like many other animals named Smart, he wants to find out the shortest path from one point to another.</p>
<p>Unfortunately, Ant Smart is not enough smart to solve this question now. It is your task to find out the answer.</p>
<h3>Input</h3>
<p>There are several test cases in this problem. The number of them is about 1000. The first line of input contains a single integer denoting the number of test cases.</p>
<p>For each test case, the first line contains two integers - the radius and height of the cylinder, separated by spaces.</p>
<p>For the next two lines, each line contains three integers: <strong>h</strong>, <strong>a</strong> and <strong>r</strong> (0 &lt;= <strong>h</strong> &lt;= height, 0 &lt;= <strong>a</strong> &lt; 360, 0 &lt;= <strong>r</strong> &lt;= radius), denoting one point on the surface of cylinder, respectively. <strong>h</strong> indicates a circle on the surface of cylinder which apart <strong>h</strong> from the bottom. And the polar angle <strong>a</strong> and radius <strong>r</strong> indicates the position of the point on the circle. In the other words, if the cylinder is (0,0,0) - (0,0,height) on the 3D grid coordinate. The point can be represented as (cos(<strong>a</strong>)*<strong>r</strong>, sin(<strong>a</strong>)*<strong>r</strong>, <strong>h</strong>).</p>
<p>You may assume that the given points must be on the surface of the given cylinder.</p>
<h3>Output</h3>
<p>For each test case, output only one line contains the length of the shortest path on the surface of cylinder. We accept solutions with absolute error less than 10<sup>-2</sup> in at least 99% of the test cases.</p>
<h3>Example</h3>
<pre><strong>Input</strong>:
2
5 10
10 0 3
5 0 5
90 49
49 312 39
0 52 65

<strong>Output:</strong>
7.00
171.02
</pre>