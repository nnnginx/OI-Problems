<p>
	Contemporary buildings can have very complicated roofs. If we take a vertical 
	section of such a roof it results in a number of sloping segments. When it is 
	raining the drops are falling down on the roof straight from the sky above. 
	Some segments are completely exposed to the rain but there may be some segments 
	partially or even completely shielded by other segments. All the water falling 
	onto a segment as a stream straight down from the lower end of the segment on 
	the ground or possibly onto some other segment. In particular, if a stream of 
	water is falling on an end of a segment then we consider it to be collected by 
	this segment.
</p>
<img alt="Rooftops" src="/content/adrian:RAIN1.png">
<p>
	For the purpose of designing a piping system it is desired to compute how much 
	water is down from each segment of the roof. To be prepared for a heavy 
	November rain you should count one liter of rain water falling on a meter of 
	the horizontal plane during one second.
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads the description of a roof,
		</li><li>
		computes the amount of water down in one second from each segment of the roof,
		</li><li>
			writes the results.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case the first line of the input contains one integer n (1 &lt;= 
	n &lt; = 40000) being the number of segments of the roof. Each of the next n 
	lines describes one segment of the roof and contains four integers x<sub>1</sub>, 
	y<sub>1</sub>, x<sub>2</sub>, y<sub>2</sub> (0 &lt;= x<sub>1</sub>, y<sub>1</sub>, 
	x<sub>2</sub>, y<sub>2</sub> &lt; = 1000000, x<sub>1</sub> &lt; x<sub>2</sub>, 
	y<sub>1</sub>&lt;&gt;y<sub>2</sub>) separated by single spaces. Integers x<sub>1</sub>, 
	y<sub>1</sub> are respectively the horizontal position and the height of the 
	left end of the segment. Integers x<sub>2</sub>, y<sub>2</sub> are respectively 
	the horizontal position and the height of the right end of the segment. The 
	segments don't have common points and there are no horizontal segments. You can 
	also assume that there are at most 25 segments placed above any point on the 
	ground level.
</p>
<h3>Output</h3>
<p>
For each test case the output consists of n lines. The i-th line should contain 
the amount of water (in liters) down from the i-th segment of the roof in one 
second.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
6 
13 7 15 6 
3 8 7 7 
1 7 5 6 
5 5 9 3 
6 3 8 2 
9 6 12 8 

<b><tt>Sample output:</tt></b>
2 
4 
2 
11 
0 
3 
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>