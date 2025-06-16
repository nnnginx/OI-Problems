<table class="problems" width="100%"><tbody><tr class="navigation">
<td width="50%"><a href="/problems/BGAME/en/">English</a></td> 
<td width="50%"><a href="/problems/BGAME/vn/">Vietnamese</a></td> 
</tr></tbody></table>


<p>Two players, A and B, play a game on a square board of size n¡Án. The squares of the board are either white or black. The game is played only on the white squares ¡ª the black ones are excluded from the game. Each player has
one piece, initially placed at this player¡¯s starting point ¡ª one of the white squares on the board. The starting point of A is different than that of B.</p>
<p>In each move a player moves his piece to one of the neighboring white squares (either up, down, left or right). If the player moves his piece to the
square currently occupied by his opponent¡¯s piece, he gets an extra move (this way he jumps over the opponent). Note that in this case the direction of the second move can be different than that of the first move. </p> <p>
Player A moves first, then players alternate. The goal of the game is to reach the opponent¡¯s starting point. The player whose piece reaches his opponent¡¯s starting point first, wins the game. Even if the player¡¯s last move consists of two jumps, and he only jumps over his opponent¡¯s starting point (since it is occupied by his opponent), the player wins. We want to determine which player has a winning strategy (a player has a winning  trategy if he can win regardless of his opponent¡¯s moves).</p>
<h3>Task</h3>
<p>
Write a program, that:</p><ul>
<li>	reads the layout of the grid and the starting points of the two players from the standard input,
</li><li>	finds the player who has a winning strategy,
</li><li>	writes the result to the standard output.
</li></ul>
<p></p>
<h3>Input</h3>
<p>The first line of the standard input contains one integer t the number of test cases (1 ¡Ü t ¡Ü 10 ). After it the description of t tests appears. Each test is described as follows. In the first line of the test there is one integer n (2 ¡Ü n ¡Ü 300 ), the length of the side of the grid. Then next n lines contain the description of the grid. Each line consists of n characters (with no whitespaces between them). Each character is either ¡¯.¡¯ a white square), ¡¯#¡¯ (a black square), ¡¯A¡¯ (the starting point of A) or ¡¯B¡¯ (the starting point of B).</p><p>

You may assume that there exists a path of white squares between the starting points of A and B.
</p>
<h3>Output</h3>
<p>For each test case exactly one line should be printed to standard output containing a single character ¡¯A¡¯ or ¡¯B¡¯, indicating the player who has a winning strategy.</p>

<h3>Example</h3>

<pre><b>Input:</b>
2
4
A...
.#..
....
...B
4
A...
....
..#.
...B


<b>Output:</b>
B
A

</pre>