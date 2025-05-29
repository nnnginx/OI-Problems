<a href="https://en.wikipedia.org/wiki/Chess">Chess</a> is a two-player strategy board game played on a <b>8 x 8</b> board. Each player begins with <b>16</b> pieces where each type of piece moves differently. Player 1 has all the white pieces and player 2 all the black ones, with white being the one to move first and then players take turns alternatingly until the game ends. The game is played on a square board of eight rows and eight columns. The rows are called ranks and are numbered 1 to 8 from bottom to top from white¡¯s perspective. Similarly, the columns are called files and are denoted from <i>a</i> to <i>h</i> from left to right according to white¡¯s perspective. The objective of the game is to threaten the opponent¡¯s king in such a way that escape is not possible, i.e, checkmate the opponent. If a player¡¯s king is threatened, it is said to be in check and the player must remove the king from check on the next move by either moving to a safe square or capturing or blocking the attacking piece(s). The figure shows the starting position for the game of chess.

<br><br>

<a href="https://cutt.ly/AcP71dv"><img src="file://KZr7arrJ.png" alt="Sample-Rank" border="0" width="300"></a>

<br><br>

In this problem, we¡¯ll be considering a slightly modified version of chess with the following rules:

<br><br>

<ol>
<li>The game will be played on a <b>N x N</b> board.</li>
<br><br>
    
<li>The game will consist of exactly 4 pieces - The white king, the black king, and two white rooks. All four pieces must be placed on different squares of the board.</li>
<br><br>
    
<li>Kings can move to any adjacent square (horizontally, vertically, or diagonally), unless the square is outside the board or occupied by a friendly piece or if the move would place the king under check.</li>
<br><br>
    
<li>Rooks can move to any square in the same rank or file, but not by jumping over other pieces. Also it cannot land on a square occupied by a friendly piece.</li>
<br><br>
    
<li>A piece <b>X</b> is threatened by another enemy piece <b>Y</b>, iff  <b>Y</b> can reach <b>X</b> in exactly one legal move.</li>
<br><br>
    
<li>A piece <b>X</b> can capture another enemy piece <b>Y</b> iff <b>X</b> can reach <b>Y</b> in exactly one legal move. On capturing, piece <b>Y</b> is removed from the board and <b>X</b> takes its place. Note that if <b>X</b> is the king, then it cannot capture <b>Y</b> if <b>Y</b> is guarded by an enemy piece. That is the king can never move and put itself in danger where it is attacked by an enemy piece.</li>
<br><br>
    
<li>The two kings cannot ever be in adjacent (horizontally, vertically or diagonally) squares.</li>
<br><br>
    

<li>The objective of the game is to place the four pieces on unique squares of the board in such a way that if it is black¡¯s move, then the black king is attacked and has no legal moves. That is, the black king must be threatened by at least one of the white rooks and has no way to move to a safe square or eliminate the checks (by capturing the attacking pieces if not guarded). Note that it is not necessary for the board configuration to be legal following the exact rules of chess. That is, if <b>N = 8</b> there might be valid configurations in our modified game which might never appear in a game of chess. Like the figure shown below, which can never occur in a proper game of chess given that it is black¡¯s turn to move, although it would be a perfectly valid configuration in our game.</li>
<br><br>

</ol>

<a href="https://cutt.ly/WcAeO08"><img src="file://P3x64Mq4.png" alt="Sample-Rank" border="0" width="300"></a>
<br><br>

Given <b>N</b>, you need to count how many ways you can place one white king, one black king, and two white rooks in the chessboard such that the black king is threatened and has no way to escape the threat given it is black¡¯s turn to move. Two configurations are different if either any of the squares contain different pieces or one square contains a piece but the other does not. Note that every square is uniquely represented by it¡¯s rank and file and hence mirrored or reversed configurations of the same configuration will be considered as different configurations. Also note that the white king, black king and white rooks are distinguishable but the two white rooks are identical. So in the figure above, if we swap the two rooks, the new configuration will be the same as the old one.
<br><br>

  
Since the number of ways can be huge, you need to output it modulo <b>7340033</b>.


<h3>Input</h3>
The first line contains the number of test cases denoted by <b>T</b>. The next <b>T</b> lines contain the board dimension <b>N</b>.
<br><br>

<h3>Constraints</h3>
<strong><li>1 ¡Ü T ¡Ü 20</li></strong>
<strong><li>1 ¡Ü N ¡Ü 10<sup>5</sup></li></strong>


<h3>Output</h3>
For each case, output one line. First output the case number then the number of valid ways modulo <b>7340033</b>. Please refer to the sample i/o for more clarity on the format.


<h3>Sample Input</h3>

<pre>8
1
2
3
4
5
6
7
8

</pre>

<h3>Sample Output</h3>
<pre>Case 1: 0
Case 2: 0
Case 3: 232
Case 4: 1432
Case 5: 5188
Case 6: 14536
Case 7: 34464
Case 8: 72392

</pre>

<h3>Explanation</h3>

For a <b>8 x 8</b> board, here are some valid configurations:
<br><br>

<a href="https://cutt.ly/McAtqFZ"><img src="file://Y8CMz88r.png" alt="Sample-Rank" border="0" width="300">
<br><br>

</a><a href="https://cutt.ly/7cAtaqH"><img src="file://TekuRIuh.png" alt="Sample-Rank" border="0" width="300"></a>
<br><br>

<a href="https://cutt.ly/qcAt2xx"><img src="file://JoRMYpgR.png" alt="Sample-Rank" border="0" width="300"></a>
<br><br>

<a href="https://cutt.ly/McAtbmF"><img src="file://deGYyzgk.png" alt="Sample-Rank" border="0" width="300"></a>
<br><br>

For all of these boards, the black king is attacked and has nowhere to go. Also both the white rooks are placed in the board and the kings are not in adjacent positions.

<br><br>
And here are some invalid ones:
<br><br>

<a href="https://cutt.ly/UcAyiJp"><img src="file://fUii2eID.png" alt="Sample-Rank" border="0" width="300">
<br><br>

</a><a href="https://cutt.ly/FcAygPS"><img src="file://jy4Z79BV.png" alt="Sample-Rank" border="0" width="300"></a>
<br><br>

<a href="https://cutt.ly/7cAyz5c"><img src="file://kjdbQAfC.png" alt="Sample-Rank" border="0" width="300"></a>
<br><br>

<a href="https://cutt.ly/2cAyQaF"><img src="file://aTSyoKMN.png" alt="Sample-Rank" border="0" width="300"></a>
<br><br>

For the first board, the black king can move and capture the attacking white rook thereby removing the check and moving to a safe square.

For the second board, although the black king is attacked and cannot capture anything because all the pieces are guarded, the two kings are adjacent which is not allowed. Hence it is not a valid checkmate position.

For the third board, it is stalemate. That is the black king has nowhere to go but it is also not attacked. So no checkmate.

For the fourth board, it is checkmate and the black king has nowhere to go. But we haven¡¯t placed both the rooks in the board and hence this is not a valid position.
<br><br>