<p>

The Bogus Corporation claims to have solved the energy crisis by devising a method to perform controlled fusion reaction! The set up consists of a cube of side length N meters, which contain K point sources of electrons. Each of the sources can be configured to emanate an electron along any of the six possible directions corresponding to +X axis, -X axis, +Y axis, -Y axis, +Z axis, -Z axis. The cube is filled with a medium in which the electrons travel with a velocity of 1m/s. At time t=0, all the sources are switched on simultaneously, emanating a single electron along the configured direction. An electron travels in a straight line until it strikes the boundary of the cube or collides with another electron. A collision between two electrons can occur in two possible ways - a head-on collision, and a side-on collision. In a head-on collision, both the electrons rebound in opposite directions with the same speed. A side-on collision occurs when the colliding electrons are travelling in mutually perpendicular directions. After a side-on collision, the colliding electrons are deflected by 90 degrees, rebounding in mutually perpendicular directions with the same speed, the plane of motion remaining the same. Note that throughout the experiment, the direction of motion of an electron remains oriented along one of the coordinate axes. If more than two electrons collide simultaneously, resolve the collision pairwise, where any two of the colliding electrons can be paired. To maximize the chances of initiating the fusion reaction, we would like to maximize the time before an electron hits a boundary wall of the cube. Given the location of the K sources, determine the orientation of the sources such that this time is maximized. Output this maximum value.

</p><h3>Input</h3>
<p>

First line contains a single integer T, the number of test cases (
1&lt;=T&lt;=50),&nbsp; followed by the description of the
test cases. The first line of each test case contains two integers, K
and N respectively ( 1&lt;=K&lt;=100,
1&lt;=N&lt;=1000). It is followed by K lines, where each line
contains space separated three integers representing the X, Y and Z
coordinates of the particular source. The coordinates of the diagonally
opposite corners of the cube are (0,0,0) and (N,N,N). All the sources
will lie strictly inside the cube.


</p><h3>Output</h3>
<p>

For each test case, output the maximum value of the time before the
first electron hits the boundary of the cube on a single line.


</p><h3>Example</h3>

<pre><b>Input:</b>
2
1 10
5 5 5
2 10
1 1 1
1 1 2
<b>Output:</b>
5
9
</pre>