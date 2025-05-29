<p><em>Original statement in spanish at <a href="http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf">http://www.dc.uba.ar/events/icpc/download/problems/taip2011-problems.pdf</a></em></p>
<p>Gabriela drives a school bus. Being one of the few women who have that job, she is always mocked by the male drivers. To improve her status, she decided that besides driving responsibly she is going to drive more efficiently. Her idea is to finish her route spending as little time as possible, without violating any traffic rule.</p>
<p>The bus Gabriela drives has a very modern driving system that allows her to adjust the acceleration to any real number instantly. Hence, the acceleration is constant by intervals, jumping to another acceleration whenever Gabriela decides so. If <em>v</em> is the bus' speed at a given instant of time, and <em>a</em> its acceleration that remains constant over a period of time <em>t</em>, then the speed at the end of that period will be <em>v + at</em>. Moreover, the bus will move a distance of <em>at<sup>2</sup>/2 + vt</em> during that period of time.</p>
<p>The traffic rules prevent vehicles from using an acceleration greater than <strong>A</strong>, or a deceleration less than <strong>D</strong>, i.e. the acceleration <em>a</em> at any time must satisfy -<strong>D</strong> &lt;= <em>a</em> &lt;= <strong>A</strong>. Moreover, there are check points along the route of the bus where the speed must lie within a certain given interval.</p>
<p>Gabriela knows in advance the location of the check points, the total length of the route, and the constants <strong>A</strong> and <strong>D</strong>. At the beginning of the route the speed and acceleration of the bus are both 0. There are no additional restrictions regarding the speed or the acceleration the bus must have at the end of the route (in particular, it is not necessary to stop in the end). Your job is to use this data to determine the minimum time that Gabriela needs in order to finish the route without violating the rules.</p>
<h3>Input</h3>
<p>The input contains several test cases. Each test case is described using several lines. The first line of each test case contains four integers <strong>N</strong>, <strong>L</strong>, <strong>A</strong> and <strong>D</strong>. <strong>N</strong> represents the total number of check points that are present in Gabriela's route (1 &lt;= <strong>N</strong> &lt;= 10<sup>5</sup>). <strong>L</strong> indicates the length of the route in meters (2 &lt;= <strong>L</strong> &lt;= 10<sup>7</sup>). <strong>A</strong> and <strong>D</strong> represent, respectively, the maximum allowed acceleration and deceleration for the bus (1 &lt;= <strong>A</strong>, <strong>D</strong> &lt;= 100). Each of the following <strong>N</strong> lines describe a different check point using three integers <strong>X</strong>, <strong>V</strong> and <strong>W</strong> that represent, respectively, the distance between the check point and the starting point of the route (1 &lt;= <strong>X</strong> &lt;= <strong>L</strong>-1), the minimum speed, and the maximum speed allowed for the bus at the time it passes by that check point (1 &lt;= <strong>V</strong>, <strong>W</strong> &lt;= 100). Assume that in each test case the check points are given in ascending order of distance from the start point of the route, and no two check points are at the same distance from the start point. In this problem, the length is expressed in m (meters), the speed in m/s, and the acceleration in m/s<sup>2</sup>. The end of the input is indicated by a line containing the number -1 four times, and should not be processed as a test case.</p>
<h3>Output</h3>
<p>For each test case, output a single line containing a rational that represents the minimum time (in seconds) needed for Gabriela to finish her route without violating any traffic rule, or an asterisk if it is impossible to do that. Round the answer to the nearest rational with two decimal digits. In case of a tie, round up. Print exactly two digits after the decimal point, even if that means ending the number with 0's.</p>
<h3>Example</h3>
<p><strong>Input:</strong></p>
<pre>1 40 10 1
20 21 21
1 40 10 5
20 20 20
1 20 10 50
10 14 15
5 1000 2 5
400 30 80
600 35 50
700 10 30
900 30 40
950 10 30
-1 -1 -1 -1
</pre>
<p><strong>Output:</strong></p>
<pre>*
2.83
2.00
35.96
</pre>