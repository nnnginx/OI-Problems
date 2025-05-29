<p>
	Solitaire is a game played on an 8x8 chessboard. The rows and columns of the 
	chessboard are numbered from 1 to 8, from the top to the bottom and from left 
	to right respectively.
</p>
<p>
	There are four identical pieces on the board. In one move it is allowed to:
</p>
<div align="justify">
	<ul>
		<li>
		move a piece to an empty neighboring field (up, down, left or right),
		</li><li>
			jump over one neighboring piece to an empty field (up, down, left or right).</li>
	</ul>
</div>
<img src="/content/adrian:solitaire.png" alt="possible moves in solitaire">
<p>
	There are 4 moves allowed for each piece in the configuration shown above. As 
	an example let's consider a piece placed in the row 4, column 4. It can be 
	moved one row up, two rows down, one column left or two columns right.
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads two chessboard configurations from the standard input,
		</li><li>
		verifies whether the second one is reachable from the first one in at most 8 
		moves,
		</li><li>
			writes the result to the standard output.</li>
	</ul>
</div>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	For each test case, each of two input lines contains 8 integers a<sub>1</sub>, 
	a<sub>2</sub>, ..., a<sub>8</sub> separated by single spaces and describes one 
	configuration of pieces on the chessboard. Integers a<sub>2j-1</sub> and a<sub>2j</sub>
	(1 &lt;= j &lt;= 4) describe the position of one piece - the row number and the 
	column number respectively.
</p>
<h3>Output</h3>
<p>
	For each test case the output should contain one word for each test case - 
	`YES' if a configuration described in the second input line is reachable from 
	the configuration described in the first input line in at most 8 moves, or one 
	word `NO' otherwise.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
4 4 4 5 5 4 6 5
2 4 3 3 3 6 4 6

<b><tt>Sample output:</tt></b>
YES
</pre>