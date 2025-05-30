<p><strong>Note: This is an easier version of the problems CSTATE2 and CSTATE3. A solution to those problems (except the I/O format) will pass here.</strong></p>
<p>&nbsp;</p>
<p>The inhabitants of Slovakistan decided to organize a national chess tournament.</p>
<p>Since the first place prize is 1 point on SPOJ, everyone played as if their life was at stake.</p>
<p>However, since time was not measured in this chess tournament (unlike at most chess tournaments in the rest of the world), a problem occured - players took way too long to admit defeat.</p>
<p>They always just kept thinking and thinking, trying to find some move which would prevent their king from being taken. Just one more moment... And perhaps one more...</p>
<p>The inhabitants of Slovakistan are planning to hold the tournament next year as well. It would be great if a skilled programmer lent them a hand and got rid of this nuisance!</p>
<p>For a given description of a chessboard, decide its state - which player's king is under threat, and whether it is a Check or a Checkmate.</p>
<p>For the purposes of this problem only take into account basic moves of every chesspiece; complicated moves such as Castling, En passant, moving a pawn 2 squares or Promotion are not accepted in Slovakistan.</p>
<h3>Input</h3>
<p>The first line of the input contains the integer <strong>1 �� t �� 2000</strong>&nbsp;- the number of chessboards. <strong>t</strong> descriptions of a chessboard follow.</p>
<p>Each description of a chessboard consists of <strong>8</strong> rows, each consisting of <strong>8</strong> characters (the chessboard is of the traditional dimensions <strong>8x8</strong>).</p>
<p>These characters are from the set <strong>{.KQRBHPkqrbhp}</strong>, representing in this order an empty square, king, queen, rook, bishop, knight (horse), and pawn.</p>
<p>The pieces belonging to the White player are marked by lowercase characters; the upper side of the chessboard (first in the input) belongs to him, hence white pawns move downwards.</p>
<p>The pieces belonging to the Black player are marked by uppercase characters; the lower side of the chessboard belongs to him, hence black pawns move upwards.</p>
<p>A blank line follows after every chessboard.</p>
<p>The number or placement of the pieces may by all means be impossible to reach in a standard game of chess, however you may assume that on every chessboard there is exactly one white king ('<strong>k</strong>') and one black king ('<strong>K</strong>').&nbsp;</p>
<h3>Output</h3>
<p>For each chessboard output one line with one of the following messages:</p>
<ul>
<li>"<strong>Safe</strong>", if neither players' kings are being threatened</li>
<li>"<strong>Impossible</strong>", if both players' kings are being threatened</li>
<li>"<strong>{colour}</strong> <strong>Check</strong>", where <strong>{colour}</strong> is either "<strong>Black</strong>" or "<strong>White</strong>", if the respective player's king is being threatened, and there exists at least one valid move by any of his pieces after which his king is no longer threatened</li>
<li>"<strong>{colour} Checkmate</strong>", where {colour} is either "<strong>Black</strong>" or "<strong>White</strong>",&nbsp;&nbsp;if the respective player's king is being threatened, and there exists no valid move by any of his pieces after which his king is no longer threatened</li>
</ul>
<h4>Additional note</h4>
<p>There are 13 input files "0" through "12".</p>
<p>In order to make finding mistakes easier and/or let you implement various chesspieces one by one, with the exception of the example (file #0), the following holds:</p>
<table border="5" cellspacing="5" cellpadding="5">
<tbody>
<tr>
<td>Chesspiece &nbsp; &nbsp;&nbsp;</td>
<td>Appears first in file #</td>
</tr>
<tr>
<td>King</td>
<td>1</td>
</tr>
<tr>
<td>Knight</td>
<td>1</td>
</tr>
<tr>
<td>Rook</td>
<td>3</td>
</tr>
<tr>
<td>Bishop</td>
<td>5</td>
</tr>
<tr>
<td>Queen</td>
<td>5</td>
</tr>
<tr>
<td>Pawn</td>
<td>8</td>
</tr>
</tbody>
</table>
<p><br>Additionally, after submission you can view extra information about the result of each file by clicking the result text ("accepted","wrong answer",...).</p>
<p>As an example, if you have received WA, the extra information looks like so:</p>
<p>File #5: Result is WA, message is 'Test Case 47: Your answer: Black Checkmate; Correct answer: Black Check', time = 0.100000, mem = 123456</p>
<p>Note that the message can go haywire if your program does something unexpected, such as end before reading all input.&nbsp;</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
7
....k...
........
...H....
........
...h....
........
....K...
........

........
....h...
..k.....
.....H..
...K....
........
........
........

k..H....
...H....
.HH.....
........
........
......K.
........
........

k..H....
...H....
.HH.....
........
........
......K.
.r......
........

K.....Rr
R.h....r
........
........
rr......
.....k..
........
........

k.......
.......R
........
...B....
.R......
......K.
..q.....
........

........
..PPP...
..PkP...
...Pp...
...K....
........
........
........</pre>
<pre><strong>Output:</strong>
Impossible
Safe
White Checkmate
White Check
Black Checkmate
White Check
Black Check</pre>
<p>This is my first time using my own judge/master judge; although this problem is 'interactive' in order to get the info message, the input is all given first before your output is read, so hopefuly it should have no effect. If you have a suspicion it is doing something funky, do let me know :)</p>