<p>
	Steve and Digit bought a box containing a number of donuts. In order to divide 
	them between themselves they play a special game that they created. The players 
	alternately take a certain, positive number of donuts from the box, but no more 
	than some fixed integer. Each player's donuts are gathered on the player's 
	side. The player that empties the box eats his donuts while the other one puts 
	his donuts back into the box and the game continues with the "loser" player 
	starting. The game goes on until all the donuts are eaten. The goal of the game 
	is to eat the most donuts. How many donuts can Steve, who starts the game, 
	count on, assuming the best strategy for both players?
</p>
<h3>Task</h3>
<p>Write a program that:</p>
<div align="justify">
	<ul>
		<li>
		reads the parameters of the game from the standard input,
		</li><li>
		computes the number of donuts Steve can count on,
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
	For each test case the first and only line of the input contains exactly two 
	integers n and m separated by a single space, 1 &lt;= m &lt;= n &lt;= 100 - the 
	parameters of the game, where n is the number of donuts in the box at the 
	beginning of the game and m is the upper limit on the number of donuts to be 
	taken by one player in one move.
</p>
<h3>Output</h3>
<p>
	For each test case the output contains exactly one integer equal to the number 
	of donuts Steve can count on.
</p>
<h3>Example</h3>
<pre><b><tt>Sample input:</tt></b>
1
5 2 

<b><tt>Sample output:</tt></b>
3
</pre>