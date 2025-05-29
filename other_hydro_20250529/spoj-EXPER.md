<p>The following experiment is taking place. There are n points of a plane. Each point is moving with the uniform velocity. It is needed to determine the minimum circle which encloses all the points after each second of the experiment during the fixed time T.

</p><h3>Input</h3>
<p>The first line of input contains the number t - the number of tests. Next comes the description of t tests. The first line of each test consists of two integers n - number of points and T - the duration of the experiment in seconds. The next n lines contain four integers separated by spaces x, y, vx, vy - initial coordinates and velocities of each point.

</p><h3>Constraints</h3>
<p>1 &lt;= t &lt;= 10<br>
1 &lt;= n &lt;= 2000<br>
1 &lt;= T &lt;= 50<br>
-100 &lt;= x, y, vx, xy &lt;= 100

</p><h3>Output</h3>
<p>For each test case print T real numbers Ri for i from 1 to T rounded to two decimals after the point. Ri should be the radius of the minimal circle which encloses all the points.

</p><h3>Example</h3>

<pre><b>Input:</b>
1
3 5
1 0 1 0
3 4 1 2
5 5 -2 -1

<b>Output:</b>
3.16
4.12
5.41
7.43
9.55

</pre>