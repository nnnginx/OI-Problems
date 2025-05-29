<p>
	An unbounded triangular grid is a plane covered by equilateral triangles:
</p>
<img src="/content/adrian:rhomb1.png" alt="rhombs">
<p>
	Two neighboring triangles in the grid form a rhomb. There are 3 types of such 
	rhombs:
</p>
<img src="/content/adrian:rhomb2.png" alt="rhombs">
<p>
	A grid polygon is a simple polygon which sides consist entirely of sides of 
	triangles in the grid. We say that a grid polygon is rhombastic if it can be 
	partitioned into internally disjoint rhombs of types A, B and C.
</p>
<p>
	As an example let's consider the following grid hexagon:
</p>
<img src="/content/adrian:rhomb3.png" alt="rhombs">
<p>
	This hexagon can be partitioned into 4 rhombs of type A, 4 rhombs of type B and 
	4 rhombs of type C:
</p>
<img src="/content/adrian:rhomb4.png" alt="rhombs">
<p>
	For a given rhombastic grid polygon P compute the numbers of rhombs of types A, 
	B and C in some correct partition.
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads a description of a rhombastic grid polygon from the standard input,
		</li><li>
		computes the numbers of rhombs of types A, B and C in some correct partition of 
		the polygon,
		</li><li>
			writes the results to the standard output.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case the first line of the input contains an integer n (3 &lt;= n 
	&lt;= 50000) - the number of sides of a rhombastic grid polygon. Each of the 
	next n lines contains a description of one side of the polygon. The sides are 
	given one by one in the clockwise order. No two consecutive sides of the 
	polygon lie on the same straight line. The description of a side consists of 
	two integers d and k. Integer d says what is the direction of the side 
	according to the following figure:
</p>
<img src="/content/adrian:rhomb5.png" alt="rhombs">
<p>
	Integer k is the length of the polygon side measured in the number of sides of 
	grid triangles. Sum of all numbers k is not larger than 100000.
</p>
<h3>Output</h3>
<p>
	For each test case the first and only line of the output contains three 
	integers separated by single spaces denoting the number of rhombs of type A, B 
	and C respectively, in some partition of the input polygon.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
6 
1 2 
2 2 
3 2 
4 2 
5 2 
6 2 

<b><tt>Sample output:</tt></b>
4 4 4
</pre>