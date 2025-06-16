<p>Garima is a student of Artifical Intelligence, she is specializing in robotics. She is designing various simulations to test run her robot algorithms. The robot works in a 1-dimensional world (which has a starting point known as origin). If a robot is 5 units away from origin, then robot is said to be at the ordinate 5. Similarly if robot is 2.5 unit away from origin, then robot is said to be at the ordinate 2.5. Robots usually operate in groups. A group of robots can be described in terms of their individual ordinates. For example, if there are three robots in a group which are present at 1.3 units, 0 units and 5 units resepectively away from origin, then we can say that the robot group is the ordered tuple &lt;1.3, 0, 5&gt;.</p>
<p>One of the attributes of the robot is it's power. Given a robot's ordinate we can determine the power of a robot using a given linear function called robot power function. Even though linear functions are of the form ax + b, but robot power functions are of the form ax and don't have any constant term. Robot's in the same group have same robot power function. For example, if robot power function is given by function f(x) = 2x, then robots in the group &lt;1.3, 0, 5&gt; have powers 2.6 units, 0 units and 10 units respectively. The average power of the group is given by (2.6 + 0 + 10)/3 = 4.2.</p>
<p>Given two robot groups (containing same number of robots), Garima wants to find robot power functions f(x) and g(x) such that f(x) = ax and g(x) = bx and 'a'&nbsp; and 'b' are positive integers and absolute difference between the average power of the two robot groups is minimized. Since 'a' and 'b' needs to be small, so a<sup>2</sup>&nbsp;+ b<sup>2</sup>&nbsp;should also be minimized.</p>
<p>More mathematically, given the robot groups &lt;x<span style="font-size: 8.33333px;"><sub>1</sub></span>, x<sub>2</sub>, ..., x<sub>n</sub>&gt; and &lt;y<sub>1</sub>, y<sub>2</sub>, .., y<sub>n</sub>&gt;, find positive integers 'a' and 'b' such that |(1/n) * ¡Æ (a*x<sub>i</sub> - b*y<sub>i</sub>)| is minimized. Since, there is a possibility that there are multiple such 'a' and 'b' so Garima puts yet another constraint of minimizing a<sup>2</sup>&nbsp;+ b<sup>2</sup></p>
<h3>Input&nbsp;</h3>
<p>The first line tells the number of test cases 't'.</p>
<p>Each test case begins with a number 'n'. 'n' corresponds to the number of robots in robot groups.</p>
<p>The next 'n' lines of the test case consist of two space seperate real numbers. For example the i<sup>th</sup>&nbsp;line contains real numbers 'x<sub>i</sub>' and 'y<sub>i</sub>' which represent the ordinates of one robot from each of the two robot groups.</p>
<p>These 'n' lines describe the two robot groups &lt;x<sub>1</sub>, x<sub>2</sub>, ..., x<sub>n</sub>&gt; and &lt;y<sub>1</sub>, y<span style="font-size: 8.33333px;"><sub>2</sub></span>, ..., y<sub>n</sub>&gt;. It is also given that not all robots in any robot group are 0 units away from origin.</p>
<p>1 &lt;= t &lt;= 100</p>
<p>1 &lt;= n &lt;= 1000</p>
<p>0 &lt; ¡Æx<sub>i</sub>&nbsp;&lt;= 10^14</p>
<p>0 &lt; ¡Æy<sub>i </sub>&lt;= 10^14</p>
<p>x<sub>i</sub> and y<sub>i</sub> can have <strong>at most 4 digits after decimal</strong>.</p>
<p>Not all of x<sub>i</sub> are zero and not all of y<sub>i</sub> are zero.</p>
<p>All x<sub>i</sub> &gt;= 0 and all y<sub>i</sub> &gt;= 0</p>
<p>#Note: x<sub>i</sub> and y<sub>i</sub> are <strong>real numbers</strong> and <strong>NOT necessarily floating-point numbers</strong></p>
<p>You can read more about floating-point numbers here: <a href="https://en.wikipedia.org/wiki/Double-precision_floating-point_format">https://en.wikipedia.org/wiki/Double-precision_floating-point_format</a></p>
<h3>Output</h3>
<p>Single line per test case.</p>
<p>Each line is of the form:</p>
<p>f(x) = ax, g(x) = bx</p>
<p>where 'a' and 'b' are the respective positive integers statisfying all the contraints given in the problem.</p>
<p>#Note: The uniqueness of 'a' and 'b' is mathematically guaranteed.</p>
<h3>Example</h3>
<pre><strong>Input:</strong></pre>
<pre>3</pre>
<pre>4</pre>
<pre>7.4 0.0027</pre>
<pre>0.022 72</pre>
<pre>0.002 0.000</pre>
<pre>0.0 0</pre>
<pre>4</pre>
<pre>8.6 0.004</pre>
<pre>0.006 0.092</pre>
<pre>0.5 0</pre>
<pre>0.002 0.004</pre>
<pre>4</pre>
<pre>25 0.73</pre>
<pre>0.0062 1.4</pre>
<pre>1 0.012</pre>
<pre>0.07 0.0000</pre>
<pre><strong>Output:</strong></pre>
<pre>f(x) = 720027x, g(x) = 74240x</pre>
<pre>f(x) = 25x, g(x) = 2277x</pre>
<pre>f(x) = 10710x, g(x) = 130381x</pre>
<pre><strong><br></strong></pre>
<pre><strong>Explanation:</strong></pre>
<pre><strong>For the first test case, we can observe that</strong><strong> </strong><strong>|(720027 * 7.4 - 74240 * 0.0027)</strong><strong> </strong><strong>+</strong><strong> </strong>(720027 * 0.022 - 74240 * 72) + (720027 * 0.002 - 74240 * 0.000) + (720027 * 0.0 - 74240 * 0)| = 0.</pre>
<pre>Since minimum absolute value can be zero so 720027 and 74240 satisfies the minimization constraint. Also, 720027 and 74240 are the smallest such values, hence they satisfy the minimization of a<sup>2</sup>+b<sup>2</sup> constraint too. </pre>
<pre> </pre>