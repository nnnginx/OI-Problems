<p>
	Consider a maze consisting of 3 rows of n square blocks each. The passageways 
	in every block match one of three possible patterns, numbered 0 (empty), 1 
	(straight) and 2 (bent), as depicted below.
</p>
<img src="/content/adrian:pattern.png" alt="Illustration of possible patterns">
<p>
	Your task is to determine whether it is possible to create a passage in a given 
	maze, with an entrance at the left end and an outlet at the right end of the 
	maze, only by rotating some of the squares of the maze by a multiple of 90 
	degrees.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	Each test case begins with a line containing a single integer n - the number of 
	squares in one row of the maze (1&lt;= n &lt;= 200000). The next n lines 
	contain three integers each, denoting the types of blocks in consecutive 
	columns of the maze. A column description is of the form <i>a b c</i> (0&lt;=<i>a,b,c</i>&lt;=2), 
	where <i>a</i> represents the type of the block in the first row, <i>b</i> - in 
	the second row and <i>c</i> - in the third row.
</p>
<h3>Output</h3>
<p>
	For each test case output the word
	<tt>yes</tt>
	if it is possible to rotate the squares so as to form a connection between the 
	left and right edge, and the word
	<tt>no</tt>
in the opposite case.
</p><p></p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
6
1 0 1
1 2 2
2 2 1
2 2 1
2 2 1
1 2 2

<b><tt>Sample output:</tt></b>
yes
</pre>
<p>Indeed, the sample input corresponds to the following maze:<br>
	<img src="/content/adrian:input.png" alt="Input illustration"><br><br>
	for which there exists a correct solution to the problem:<br>
	<img src="/content/adrian:output.png" alt="Illustration of the solution">
</p>
<b>Warning: large Input/Output data, be careful with certain languages</b>