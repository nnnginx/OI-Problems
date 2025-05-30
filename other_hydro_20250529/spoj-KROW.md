<p>Hansel and Gretel do not listen to their teacher at school. Instead they secretly play a game called K-In-A-Row. One day in the evening they started to argue who had won more games that day. They collected all the papers they had used for playing the game and they started to count how many times each of them had won. But it was very tedious and they were sleepy. Help them to count how many games each of them had won.</p>
<p>K-In-A-Row is played in a square grid with M times N squares. Two players alternate in their moves. A player chooses an empty square and fills in his/her sign (Hansel uses cross 'x' and Gretel uses circle 'o'). The game is won by the player who first places at least K his/her own signs in a row (either horizontally, vertically or in one of the two diagonal directions). The game stops immediately after one of the players completes K of his/her signs in a row; thus it may never happen that both players have completed K of their signs in a row. If no player creates such a row, nobody wins.</p>
<h3>Input file specification</h3>
<p>The first line contains the number of games L. It is followed by L blocks, each describing one game. Each block starts with a line containing 3 numbers M, N and K. Numbers M and N give the size of the grid (M,N&lt;200) and K is the length of the required row. The following N lines each containing M characters describe the situation after the end of the game. Character '.' denotes an empty field, characters 'x' and 'o' denote fields marked by Hansel and Gretel respectively. You may assume that the input is correct.</p>
<h3>Output file specification</h3>
<p>The output file consists of two numbers separated by a colon ':'. The first number denotes the number of the games won by Hansel, the second one gives the number of the games won by Gretel.</p>
<h3>Example</h3>
<pre><strong>Input file:</strong>
2
3 3 3
.x.
.xo
oox
4 7 4
....
..x.
ooox
oxx.
oox.
o.ox
..xx

<strong>Output file: </strong>
0:1
</pre>