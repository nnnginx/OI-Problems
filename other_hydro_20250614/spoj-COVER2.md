<p>In the 3D Cartesian coordinate system, there are n cubes.These cubes are all axis-paralleled. What's the volume of the union of these cubes?</p>
<h3>Input</h3>
<p>There is a single integer m in the very first line of the input, the number of test cases. m blocks follow.</p>
<p>For each test, the first line contains a single integer n(1&lt;=n&lt;=100), the number of cubes. n lines follow, each contains four integers x,y,z,r(-1000&lt;=x,y,z&lt;=1000,1&lt;=r&lt;=200), separated by spaces.
x,y,z are the X,Y,Z coordinates of the center of the  cube, and r is the distance between the center and any surface of the cube.</p>
<h3>Output</h3>
<p>m lines,each contains a single integer - the answer.</p>
<h3>Example</h3>
<pre><b><tt>Sample Input:</tt></b>
1
3
0 0 0 3
1 -1 0 1
19 3 5 6
<b><tt>Sample Output:</tt></b>
1944
</pre>