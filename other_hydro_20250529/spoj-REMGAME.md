<p>
Consider the following game. The game is played on a  5 x 5 board.  Initially  every  array  cell  has  a  piece 
in  it.  Two players  remove pieces alternatively  from  the  board.  The player  can  remove  any  number  of  consecutive pieces  in a row or column.
For example,  in  the configuration depicted below where one  indicates  a 
piece,  the  player  can  either  remove  one  piece  (<b>A1</b>, <b>A2</b>,  or 
<b>B1</b>),  or remove two pieces (<b>A1</b> and <b>A2</b>, or <b>A1</b> and
<b>B1</b>) simultaneously. The game ends when one player is forced to take the
last piece, and the other player wins the game.

</p><p>

</p><p>
<br>

</p><div align="CENTER">
<table cellpadding="3" border="1">
<tbody><tr><td align="CENTER">&nbsp;</td>
<td align="CENTER"><b> 1</b></td>
<td align="CENTER"><b> 2</b></td>
<td align="CENTER"><b> 3</b></td>
<td align="CENTER"><b> 4</b></td>
<td align="CENTER"><b> 5</b></td>
</tr>
<tr><td align="CENTER"><b> A</b></td>
<td align="CENTER">1</td>
<td align="CENTER">1</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
</tr>
<tr><td align="CENTER"><b> B</b></td>
<td align="CENTER">1</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
</tr>
<tr><td align="CENTER"><b> C</b></td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
</tr>
<tr><td align="CENTER"><b> D</b></td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
</tr>
<tr><td align="CENTER"><b> E</b></td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
<td align="CENTER">0</td>
</tr>
</tbody></table></div>

<p>

</p><p>
<br>
Write  a  program  that  evaluates  board  configurations  from  this  game.  
The  program must  output  "winning" when there exists a winning move
that no matter how the opponent responds, it will force the opponent to take
the last piece. Otherwise, the program must output "losing". 

</p><h3>Input</h3>
<p> 
The first line contains <b>n</b>, the number
of test cases.  For each test case, a 5x5 grid
of an initial game configuration is shown.
</p><h3>Output</h3>
<p>
For each case, output "winning" or "losing".

</p><h3>Example</h3>

<pre><b>Input:</b>
1 
1 0 0 0 0 
1 1 0 0 0 
1 1 1 0 0 
1 1 1 1 0 
1 1 1 1 1

<b>Output:</b>
winning
</pre>