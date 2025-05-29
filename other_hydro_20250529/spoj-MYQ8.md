<p>Prasanna and Nithin had mastered Thuvax's national game, <a href="http://en.wikipedia.org/wiki/Tic-tac-toe" target="_blank">TicTacToe</a>. <br>&nbsp;<br>TicTacToe is a board game for two players, x and o, who take turns (alternatively) marking the spaces in a 3¡Á3 grid with their signs 'x' and 'o' respectively. The x player goes first. The player who succeeds in placing three of his signs in a horizontal, vertical, or diagonal row wins the game and the game stops there.</p>
<p>While returning from a TicTacToe tournament, Prasanna and Nithin find a tictactoe like grid. They decide to continue playing from the state the board was in. Help Nithin find whether the next person to move will win/lose or whether the game will result in a tie (assuming both players play optimally), or if such a state is invalid.</p>
<h3>Input</h3>
<p>First line of the input contains a number T (1&lt;=T&lt;=10^6), followed by 4*T lines. The first line of each testcase is empty and the next 3 lines show the state of the game.</p>
<h3>Output</h3>
<p>Print win/lose/tie/invalid for each testcase on a separate line.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3 <br>&nbsp;<br>oox <br>.x. <br>..x <br>&nbsp;<br>xox <br>xoo <br>oxx <br>&nbsp;<br>o.. <br>... <br>...

<strong>Output:</strong>
lose <br>tie <br>invalid<br><br>Explanation: <br>Case 1: Player x can win by placing x in either last cell of the middle row, or the first cell of the last row. So the next player, o, cant prevent him from winning from this state. <br>Case 2: It is completed game, as you can see no one has won. So, it has ended in a tie. <br>Case 3: Player x should have started the game. Hence such a state can never be reached.</pre>