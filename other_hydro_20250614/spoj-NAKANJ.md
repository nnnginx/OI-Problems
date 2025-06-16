<p>Anjali and Nakul are good friends. They both had a quarrel recently while playing chess. Nakul wants to know the minimum number of moves a knight takes to reach from one square to another square of a chess board (8X8). Nakul is brilliant and he had already written a program to solve the problem. Nakul wants to know whether Anjali can do it. Anjali is very weak in programming. Help her to solve the problem.</p>

<p>A knight can move in the shape of an "L" in a chessboard - two squares either forward, backward, left, or right and then one square to its left or right. A knight move is valid if it moves as mentioned above and it is within the boundary of the chessboard (8 X 8).</p>

<!--
<p><center><img src="http://0.tqn.com/d/chess/1/0/6/-/-/-/KnightMoves.gif" alt="http://0.tqn.com/d/chess/1/0/6/-/-/-/KnightMoves.gif" width="400" /></center></p>
Old image link - broken
-->
<p><img title="knight" src="../../content/francky:knight" alt="knight" width="50%"></p>
<h3>Input</h3>
<p>There are T test cases in total. The next T lines contain two strings (start and destination) separated by a space.</p>
<p>The strings start and destination will only contain two characters -  First character is an alphabet between 'a' and 'h' (inclusive), Second  character is a digit between '1' and '8' (inclusive) - (Quotes just for  clarity).</p>
<p>To know the knight moves more clearly refer to the above figure.</p>

<h3>Output</h3>
<p>Print the minimum number of moves a knight takes to reach from start to destination in a separate line.</p>

<h3>Constarints</h3>
<p>1 &lt;= T &lt;= 4096</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
3
a1 h8
a1 c2
h8 c3

<strong>Output:</strong>
6
1
4</pre>