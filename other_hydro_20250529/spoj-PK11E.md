<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/PK11E/en/">English</a></td>
<td width="50%"><a href="/problems/PK11E/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">Queen game is played in a chessboard of size R rows and C columns. Rows are numbered from 1 to R and columns are numbered from 1 to C. The topmost square is in row 1 and column 1. The game is a 2 player game. Initially there are N queens placed in various squares of the chessboard. In his turn, the player picks a queen and moves it either towards the top vertically, or towards the left horizontally or towards the top-left diagonally and the queen should always stay on the board. When the queen reaches square (1, 1) it is removed from the board. The player who gives the last move wins. Each square is big enough to accommodate infinite number of queens. The players give their moves by turns. You are given the size of the chessboard and the initial positions of the N queens. Assuming that both of the players play perfectly your task is to determine who will win this game.&nbsp;</span></p>
<h3>Input</h3>
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">First line of the input contains T the number of test cases. Each test case starts with a line containing 3 integers R(1¡ÜR¡Ü25), C(1¡ÜC¡Ü10<sup>15</sup>) and N(1¡ÜN¡Ü1000). Each of the next N lines contains the positions of N queens. The position is denoted by two integers. The first integer is the row number and the second integer is the column numbers.&nbsp;</span></p>
<h3>Output</h3>
<p><span style="font-size: 12.000000pt; font-family: 'TimesNewRomanPSMT';">For each test case output ¡°YES¡± if the first player has a winning strategy and ¡°NO¡± otherwise. Look at the output for sample input for details.&nbsp;</span></p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">3&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">5 5 1&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">2 3&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">5 5 2&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">4 4&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">4 4&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">5 5 3&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">1 2&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">2 1&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">2 2&nbsp;</span></p>

<strong>Output:</strong>
<p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">NO&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">NO&nbsp;</span></p><p><span style="font-size: 12.000000pt; font-family: 'CourierNewPSMT';">YES&nbsp;</span></p></pre>
<p> </p>