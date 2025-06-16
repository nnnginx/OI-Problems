<p>
	Everyone loves gambling in the Dicent City. Every Saturday the whole community 
	meets to attend a dice contest. They started a few years ago with a classic 
	six-sided die with 1 to 6 dots displayed on the sides and had a lot of fun.
</p>
<img alt="A die" src="/content/john_jones:dice1.jpg">
<p>
	However they soon got bored and that's why more sophisticated dice are in use 
	nowadays. They put a sticker on each side and write a positive integer on each 
	sticker.
</p>
<p>
	The contest is run on a strip divided into squares in a chessboard-like manner. 
	The strip is 4 squares wide and infinite to the left and to the right (is 
	anyone going to say it can't exist in the real world, huh?). The rows of the 
	strip are numbered from 1 to 4 from the bottom to the top and the columns are 
	numbered by consecutive integers from the left to the right. Each square is 
	identified by a pair (x,y) where x is a column number and y is a row number.
</p>
<p>
	The game begins with a die placed on a square chosen be a contest committee 
	with one-dot side on the top and two-dots side facing the player. To move the 
	die the player must roll the die over an edge to an adjacent (either 
	horizontally or vertically) square. The number displayed on the top of the die 
	after a roll is the cost of the move. The goal of the game is to roll the die 
	from the starting square to the selected target square so that the sum of costs 
	of all moves is minimal.
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads the description of a die, a starting square and a target square,
		</li><li>
		computes the minimal cost of rolling the die from the starting square to the 
		target square,
		</li><li>
			writes the result.</li>
	</ul>
</div>
<p>
	Note: all teams participating in the contest received dice from the organisers.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
For each test case the first line of the input contains six integers l<sub>1</sub>, l<sub>2</sub>, 
l<sub>3</sub>, l<sub>4</sub>, l<sub>5</sub>, l<sub>6</sub> (1 &lt; = l<sub>i</sub>
&lt; = 50) separated by single spaces. Integer l<sub>i</sub> is the number 
written on a side having originally i dots. The second line of the input 
contains four integers x<sub>1</sub>, y<sub>1</sub>, x<sub>2</sub>, y<sub>2</sub>
( -10<sup>9</sup> &lt; = x<sub>1</sub>, x<sub>2</sub> &lt; = 10<sup>9</sup>, 1 
&lt;= y<sub>1</sub>, y<sub>2</sub> &lt; = 4) separated by single spaces. 
Integers x<sub>1</sub>, y<sub>1</sub> are the column and the row number of the 
starting square respectively. Integers x<sub>2</sub>, y<sub>2</sub> are the 
column and the row number of the target square respectively.
</p>
<h3>Output</h3>
<p>
For each test case the first and the only line of the output should contain the 
minimal cost of rolling the die from the starting square to the target square.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
1 2 8 3 1 4 
-1 1 0 2 

<b><tt>Sample output:</tt></b>
7 
</pre>