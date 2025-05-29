<p>
	There is a number of disjoint vertical line segments in the plane. We say that 
	two segments are horizontally visible if they can be connected by a horizontal 
	line segment that does not have any common points with other vertical segments. 
	Three different vertical segments are said to form a triangle of segments if 
	each two of them are horizontally visible. How many triangles can be found in a 
	given set of vertical segments?
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads the description of a set of vertical segments,
		</li><li>
		computes the number of triangles in this set,
		</li><li>
			writes the result.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The first line of the input contains exactly one positive integer d equal to 
	the number of data sets, 1 &lt;= d &lt;= 20. The data sets follow.
</p>
<p>
The first line of each data set contains exactly one integer n, 1 &lt;= n &lt; 
= 8000, equal to the number of vertical line segments.
</p><p>
	Each of the following n lines consists of exactly 3 nonnegative integers 
	separated by single spaces: y'<sub>i</sub>, y''<sub>i</sub>, x<sub>i</sub>(that 
	is the y-coordinate of the beginning of a segment, y-coordinate of its end and 
	its x-coordinate, respectively). The coordinates satisfy: 0 &lt; = y'<sub>i</sub>&lt; 
	y''<sub>i</sub> &lt;= 8000, 0 &lt; = x<sub>i</sub> &lt;= 8000. The segments are 
	disjoint.
</p>
<h3>Output</h3>
<p>
	The output should consist of exactly d lines, one line for each data set. Line 
	i should contain exactly one integer equal to the number of triangles in the 
	i-th data set.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1 
5 
0 4 4 
0 3 1 
3 4 2 
0 2 2 
0 2 3 

<b><tt>Sample output:</tt></b>
1 
</pre>