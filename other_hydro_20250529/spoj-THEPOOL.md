<p>A set of N billiard balls are set on a one-dimensional table. The table is 10<sup>5</sup> meters long, with two pockets at either side. Each ball has zero width and there is no friction so it is moving with a fixed velocity of either left or right and bounces back in a <a href="http://en.wikipedia.org/wiki/Elastic_collision">perfect elastic collision</a> from other balls it encounter on its way (or drop into one of the pockets). Your job is to keep track of the balls' movements.</p>
<h3>Input</h3>
<p>The first number, N, is the number of balls (&lt;= 10<sup>5</sup>).</p>
<p>This is followed by N pairs of numbers: the distance in meters from the left end of the table and the velocity (positive speed meaning it moves towards right).</p>
<p>The next line tells you which ball you have to track ( 1 &lt;= tracked ball &lt;= N).<br>The last line tells you the time T at which you have to locate the tracked ball.</p>
<p>Note: Each number is on a separate line.</p>
<h3>Output</h3>
<p>You have to output the position (from the left end) of the tracked ball after time T.</p>
<h3>Example 1</h3>
<pre><strong>Input:</strong>
1 <br>50 <br>1 <br>1 <br>6

<strong>Output:</strong>
56<br></pre>
<h3>Example 2</h3>
<pre><strong>Input:</strong>
2 <br>95<br>-1 <br>10 <br>1 <br>1 <br>60

<strong>Output:</strong><br>35<br><br><pre>Explanation : <br>2 is the number of balls,<br>One ball is placed at 95 from the left end. It's velocity is -1 (i.e. 1 m/s towards left).<br>Another ball is at distance 10. Velocity is 1 (i.e. towards right).<br>The first ball from left end is to be tracked. (i.e. ball at distance 10 from left end).<br>You need to find the new position of the tracked ball at time t=60s.</pre>
</pre>