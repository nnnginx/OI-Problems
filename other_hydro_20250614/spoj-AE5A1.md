<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/AE5A1/en/">English</a></td>
<td width="50%"><a href="/problems/AE5A1/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>In the ¡±circular game¡± the board consists of m fields arranged on a circle and numbered from 1 to m. On the board there are b white and c black pieces, at most one on each field. Two players are playing the game, the white player and the black player. Starting from the white player, the players perform their moves on the board alternately. A move consists of moving a piece of the player¡¯s colour any number of free fields forward or backward. For instance, for the board depicted below, the white player can move the piece from field 3 to field 4 or the piece from field 8 to any of the fields 7, 9 and 1.</p>
<p><img src="./21265/file/6SXBkEbo.png" alt=""></p>
<p>If a player can perform no moves in his turn, he loses. Knowing that both players play optimally, check who wins the game. It can happen that none of the players wins (the game never ends).</p>
<h3>Input</h3>
<p>The first line of the standard input contains one integer t representing the number of boards to be considered.</p>
<p>The following lines contain descriptions of respective boards, each of which consists of three lines. In the first line there are three integers m, b and c (1 ¡Ü m ¡Ü 10<sup>9</sup>, 1 ¡Ü b, c) separated by single spaces and denoting the length of the board, the number of white pieces and the number of black pieces. In the second line there is an increasing sequence of b integers (in the range 1, . . . ,m) representing the positions of white pieces. In the third line there is an increasing sequence of c integers (in the range 1, . . . ,m) representing the positions of black pieces. The total number of pieces in all boards does not exceed 10<sup>6</sup>.</p>
<h3>Output</h3>
<p>Exactly t lines with answers for consecutive boards should be written to the standard output. The answer is always a single character: B, C, or R, depending on whether the white player wins (B), the black player wins (C) or the game never ends (R).</p>
<h3>Example</h3>
<p>For the input data:</p>
<pre>3
9 2 3
3 8
2 5 6
6 2 2
5 6
2 4
7 1 1
3
4
</pre>
<p>the correct result is:</p>
<pre>C
B
R
</pre>
<p> </p>