<p>
	On the rectangular chessboard of n x m square fields we choose one field 
	adjacent to the edge of the chessboard, called the starting field. Then we put 
	a ball in the center of this field and push it to roll through the chessboard. 
	The diameter of the ball equals the width (and height) of chessboard field. The 
	angle between the direction of ball movement and the edge of the chessboard 
	equals 45 degrees. The ball bounces off the edges of the chessboard: if the 
	ball touches the edge of the chessboard then each composite of its velocity 
	perpendicular to the edge touched is reversed. At the start the ball is pushed 
	toward increasing coordinates (when the starting field is a field of the 
	highest coordinate, the ball bounces momentarily).
</p>
<p>
	We assign a point to a field of the chessboard each time the point of adjacency 
	between the ball and the chessboard enters the interior of the field. The game 
	is over when a point is assigned to the starting field. What is the number of 
	fields to which an odd number of points is assigned? The following figures 
	illustrate the problem. The route of the ball is marked with a dashed line. 
	Fields with the odd number of points are shadowed.
</p>
<img width="600" src="/content/adrian:ball1.png">
<h3>Task</h3>
<p>
	Write a program which for each data set from a sequence of several data sets:
	</p><div align="left">
		<ul>
			<li>
			reads the dimensions of the chessboard and the coordinates of starting field 
			from input,
			</li><li>
			computes the number of fields with the odd number of points,
			</li><li>
			writes the result to output.
		</li></ul>
	</div>
<p></p>
<h3>Input</h3>
<p>
	The first line of the input file contains one integer d, 1 &lt;= d &lt;= 10, which is 
	the number of data sets. The data sets follow. Each data set occupies one line 
	of the input file. Such a line consists of four integers x, y, a, b separated 
	with single spaces. These integers are the x- and y-dimensions of the 
	chessboard and x- and y-coordinates of the starting field, respectively. 
	Integers x and y are greater than two, the number of fields of the chessboard 
	does not exceed 10<sup>9</sup>,the starting field is adjacent to the edge of 
	the chessboard.
</p>
<h3>Output</h3>
<p>
The i-th line of output should contain one integer which is equal to the number 
of fields of the chessboard with the odd number of points. </p>
<h3>Example</h3>
<pre>Sample input:

2
13 6 1 5
10 7 1 5

Sample output:

2 
22
</pre>