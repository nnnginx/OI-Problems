<p>Tic Tac Toe is a child's game played on a 3 by 3 grid. One player, X, starts by placing an X at an unoccupied grid position. Then the other player, O, places an O at an unoccupied grid position. Play alternates between X and O until the grid is filled or one player's symbols occupy an entire line (vertical, horizontal, or diagonal) in the grid.

</p><p><br>We will denote the initial empty Tic Tac Toe grid with nine dots. Whenever X or O plays we fill in an X or an O in the appropriate position. The example below illustrates each grid configuration from the beginning to the end of a game in which X wins.

</p><p><br>
</p><center><img src="/content/steinersp:tictactoe.png" alt="subir imagenes" border="0"></center>
<p><br><br>

Your job is to read a grid and to determine whether or not it could possibly be part of a valid Tic Tac Toe game. That is, is there a series of plays that can yield this grid somewhere between the start and end of the game?

</p><p><br>
</p><h3>Input</h3>
<p>The first line of input contains N, the number of test cases. 4N-1 lines follow, specifying N grid configurations separated by empty lines.

<br>
</p><h3>Output</h3>
<p>For each case print "yes" or "no" on a line by itself, indicating whether or not the configuration could be part of a Tic Tac Toe game.

</p><h3>Example</h3>

<pre><b>Input:</b>
2
X.O
OO.
XXX

O.X
XX.
OOO

<b>Output:</b>
yes
no
</pre>