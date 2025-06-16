<p>A shepherd is having some trouble penning in his flock of sheep. After several 
	hours of ineffectual efforts he gives up, with some of the sheep within their 
	polygon-shaped pen and some outside. Exhausted, he moves to a place within the 
	pen from which he can see the whole interior of the pen (without any fence 
	getting in the way) and begins to count the sheep which are within it. Please 
	assist him in his task.
</p>
<h3>Input</h3>
<p>The input begins with the integer t, the number of test cases. Then t test cases 
	follow.
</p>
<p>The first line of each test case contains two integers n m, denoting the number 
	of vertices of the polygon forming the fence, and the number of sheep in the 
	whole herd (3&lt;=n&lt;=100000, 0&lt;=m&lt;=100000). The next n lines contain 
	two integers each, the i-th being x<sub>i</sub> y<sub>i</sub> - the x and y 
	coordinates of the i-th vertex of the fence (given in anti-clockwise order, 
	-32000&lt;=x<sub>i</sub>,y<sub>i</sub>&lt;=32000). The next m lines contain two 
	integers each, the j-th being x<sub>j</sub> y<sub>j</sub> - the x and y 
	coordinates of the j-th sheep (arranged in decreasing order of seniority, 
	-32000&lt;=x<sub>j</sub>,y<sub>j</sub>&lt;=32000). The shepherd's observation 
	point is within the pen and has coordinates (0,0).
</p>
<h3>Output</h3>
<p>For each test case output a line with a single integer - the number of sheep 
	within the pen. The sheep which are sitting back on the fence and enjoying a 
	cigarette should be included in the count.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
6 5
2 2
4 4
6 6
-3 1
-1 -1
5 1
2 1
3 2
6 6
3 3
-3 0

<b><tt>Sample output:</tt></b>
3
</pre>
<p>Illustration of the sample test data:<br>
	<br>
	<img src="/content/adrian:sheep.png" alt="The sheep with their shepherd">
</p>
<b>Warning: large Input/Output data, be careful with certain languages</b>