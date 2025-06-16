<p>
	<i>The loner</i> is a one-dimensional board game for a single player. The board 
	is composed of squares arranged in a single line, some of which initially have 
	pawns on them. The player makes a move by jumping with a pawn over a pawn on an 
	adjacent field, to an empty square two fields to the right or left of its 
	initial position. The pawn that was jumped over is removed directly after the 
	move, as illustrated below.
</p>
	<img src="/content/adrian:move.png" alt="The two acceptable types of moves">
<p>
	The game is considered won if exactly one pawn remains on the gaming board, and is lost if the player cannot make a move.
</p>
<p>
	Given the initial state of the gaming board, your task is to determine whether 
	it is possible for the player to win the game.
</p>
<h3>Input</h3>
<p>
	The input begins with the integer t, the number of test cases. Then t test 
	cases follow.
</p>
<p>
	Each test cases begins with the positive integer n &lt;= 32000, denoting the 
	size of the gaming board. The second and last line of the test case description 
	contains a sequence of n characters 0 or 1, without any white spaces. The i-th 
	square of the board is occupied by a pawn at the start of the game iff the i-th 
	character of this sequence is 1.
</p>
<h3>Output</h3>
<p>
	For each test case output the word <tt>yes</tt> if it is possible for the 
	player to win the game for the presented starting configuration, or the word <tt>no</tt>
	in the opposite case.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
2
7
0110011
6
111001

<b><tt>Sample output:</tt></b>
yes
no
</pre>