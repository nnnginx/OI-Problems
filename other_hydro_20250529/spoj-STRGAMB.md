<p>Madrid is a tremendously historic and monumental city that attracts several millions of visitors each year. Where there are tourists, there are also artists that entertain the crowds in the streets and gamblers that challenge pedestrians to often snaky games. One of them is just about to ask you for a game. Although you learned in problem X some basics of Spanish conjugation, you are not proficient enough to understand the rules of the game. This is why you decide to observe first some games, from which you succeede to extract the rules correctly:</p>
<table border="0">
<tbody>
<tr>
<td style="border-style: solid; border-width: 1px; text-align: center;">1</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">2</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">3</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">4</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">5</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">6</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">7</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">8</td>
</tr>
<tr>
<td style="border-style: solid; border-width: 1px; text-align: center;">&nbsp;</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">&nbsp;</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">O</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">&nbsp;</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">O</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">O</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">O</td>
<td style="border-style: solid; border-width: 1px; text-align: center;">O</td>
</tr>
</tbody>
</table>
<p>It is a two player game and players take alternate turns on a board with squares numbered from 1 to N. Some of the squares contain one Spanish 1 cent coin, others don¡¯t. At each turn, the player has to select one square containing a coin and removes the coin from the square, leaving that square empty. At the same time this player may, if he wishes so, select a second square to the left from the first one. In the left square, the player is allowed either to put 1 coin if this square is empty or to empty that box in case it contained a coin. The game finishes when there is no coin left on the board and the player to make the last move wins. <br><br>Here are the turns you observed for the initial game constellation of the above figure:</p>
<pre>XXOXOOOO&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Tourist empties 7 and puts a coin in 4<br>XXOOOOXO&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Gambler empties 8 as well as 4<br>XXOXOOXX&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Tourist empties 6 and puts a coin in 1<br>OXOXOXXX&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Gambler empties 5 and puts a coin in 2<br>OOOXXXXX&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Tourist empties 1<br>XOOXXXXX&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Gambler empties 3 as well as 2<br>XXXXXXXX&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Tourist lost the game, as no coin is left</pre>
<p>You are a bit surprised that the gambler wins most of the games. He must indeed have several years of experience and know some tricks. As you are smart, you discover his trick. Supposing that both of you play optimally, that is, once you are in a winning constellation, <br><br>you¡¯ll find the correct moves to win the game, can you tell for a given constellation whether you should make the first move or leave it to the gambler? Of course you want to win!</p>
<h3>Input</h3>
<p>The input consists of several test cases (T300), one per line that describes the initial board constellation as a string of ¡®O¡¯s and ¡®X¡¯s. Read from left to right, this string describes the board constellation from position 1 to position N (N255). ¡®O¡¯ stands for a square with coin, ¡®X¡¯ for an empty square. The input terminates on the string ¡°end¡± that should obviously not be processed.</p>
<h3>Output</h3>
<p>Output ¡°I¡¯d like to play first¡± or ¡°After you¡±, so that you will win the game.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>XXOOOX<br>OOOXX<br>XOOOOOOOO<br>XXXXOXXXXXXXOXOXXXXXXOXXXXXXXXX<br>end<br><br><strong>Output:</strong><br>I'd like to play first<br>After you<br>After you<br>I'd like to play first<br></pre>