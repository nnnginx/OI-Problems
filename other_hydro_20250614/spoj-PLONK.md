<p>
	Consider a city bounded by a square, whose n horizontal and n vertical streets 
	divide it into (n+1)<sup>2</sup> square blocks. However, in tribute to the 
	ancient traditions of the first dwellers (who tended to overindulge in 
	alcohol), all the inhabitants live at crossroads. A group of friends would like 
	to meet for an evening of merriment at the place of residence of one of them. 
	With a good deal of foresight, anticipating the difficulties they might have 
	getting back to their respective homes, they would like to meet in the house of 
	the friend which minimises the total walking distance for all of them. Assume 
	that everybody walks along the streets, turning only at crossroads, and the 
	distance between&nbsp;any pair of&nbsp;adjacent crossroads is 1.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case the first line of input contains the integer n - the number 
	of friends who want to meet (1&lt;=n&lt;=10000). The next n lines contain two 
	integers each, the i-th being x<sub>i</sub> y<sub>i</sub>, standing for the x 
	and y coordinates of the crossroads at which the i-th friend lives (0&lt;=x<sub>i</sub>,y<sub>i</sub>&lt;=100000).
</p>
<h3>Output</h3>
<p>
	For each test case output the total distance covered by all friends when 
	walking to the meeting place.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
7
1 3
3 2
3 5
6 9
10 1
12 4
5 7

<b><tt>Sample output:</tt></b>
39
</pre>
<b>Warning: large Input/Output data, be careful with certain languages</b>