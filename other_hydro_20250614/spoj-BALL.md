<p>In a coordinate plane, there are N horizontal conveyor belts, each moving either leftwards or rightwards. When the ball falls on a belt, the belt drags it in direction it's moving. When the ball reaches the end of the belt, it falls vertically downwards. For example, if the belt is moving rightwards and it ends in the unit square with x-coordinate 12, the ball will fall from the belt on the x-coordinate 13, and continue falling on the same x-coordinate until it falls on another belt or reaches the ground (the height of 0).</p>
<p>Frane drops a ball many times (from the height that is greater than any of the belt heights), from various x-coordinates, and your task is: for each ball Frane drops, determine the direction of each belt such that this ball falls on as many belts as possible.</p>
<p>This picture reprezents the first test example: &nbsp;<img title="First example" src="file://Q4gNPUBp.png" alt="" width="211" height="161"></p>
<h3>Input</h3>
<p>In the first line of input, there is an integer N (the number of conveyor belts, 1 ¡Ü N ¡Ü&nbsp;100000).</p>
<p>In each of the next N lines, there are integers X1, X2, Y (X1 ¡Ü&nbsp;X2, 0 &lt; X1, X2, Y &lt; 10<sup>9</sup>) reprezenting the belt. Imagine the belt as a segment of which the bounding unit squares are (X1, Y) and (X2, Y). The belt's thickness is zero and it lies on the bottom of the given unit squares. The belts will not touch or overlap each other.</p>
<p>In the next line, there is an integer Q (the number of falling balls, 1 ¡Ü Q ¡Ü&nbsp;100000).</p>
<p>In the next Q lines there is an integer less than 10<sup>9</sup>, reprezenting the x-coordinate of the unit square Frane drops the ball from.</p>
<h3>Output</h3>
<p>For each of the Q queries, output the greatest possible number of the conveyor belts visited by the ball.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px;">3
1 4 3
5 7 2
2 4 1
4
1
4
5
6</pre>
<strong>Output:</strong></pre>
<pre>3</pre>
<pre>3</pre>
<pre>2</pre>
<pre>2</pre>
<pre><strong>Input:</strong></pre>
<pre><pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px; font-weight: bold;">3
5 20 20
15 30 15
10 14 11
3
5
30
516546</pre>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px; font-weight: bold;"><strong><strong>Output:</strong></strong></pre>
<pre style="font-family: 'Courier New', Courier, monospace; font-size: 12px; font-weight: bold;"><pre style="color: #000000; font-family: 'Courier New', Courier, monospace; font-size: 12px; font-weight: bold; margin: 8px;">3
2
0</pre>
<strong> </strong></pre>
</pre>