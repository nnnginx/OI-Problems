<p>Consider a rectangular snooker table with pockets only at the 4 corners of the rectangle as shown in the image below. Consider all integer points on the boundary of the table. At each point, except the four corners (four pockets), you are allowed to hit the ball at an angle of <strong>45</strong> degrees from the side of the table from which you are hitting the ball.</p>
<p>From any point on the boundary you can hit the ball in two directions and they are considered to be two different ways. For instance in the image shown below, from the point S the ball can be hit in two ways as shown.</p>
<p>Given the dimensions of the board your task is to find the number of ways in which the ball can be hit so that it <em>eventually</em> reaches one of the four holes.</p>
<p>Consider the ball to be of negligible size, like a point. Also assume that the ball does not lose energy due to collisions or friction - it keeps moving until it drops into a hole.</p>
<p><img src="../../../content/swarnaprakash:snooker.jpg" alt=""></p>
<h3>Input</h3>
<p>The input has multiple test cases. Each test case consists of two space separated integers <strong>M</strong> and <strong>N</strong>, 2 ¡Ü M,N ¡Ü 10^5, representing the dimensions of the table. M=N=0 indicates the end of tests. There are atmost 300 testcases.</p>
<h3>Output</h3>
<p>For each test case output the number of ways as described, in a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2 2
2 4
3 5
0 0

<strong>Output:</strong>
0
4
24

</pre>