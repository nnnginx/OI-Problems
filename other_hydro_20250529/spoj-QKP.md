<p>
You all are familiar with the famous 8-queens problem which asks you to place 8 queens on a chess
board so no two attack each other. In this problem, you will be given locations of queens and knights
and pawns and asked to find how many of the unoccupied squares on the board are not under attack
from either a queen or a knight (or both). We¡¯ll call such squares ¡°safe¡± squares. Here, pawns will
only serve as blockers and have no capturing ability. The board below has 6 safe squares. (The shaded
squares are safe.)

</p><p>
</p><center><img src="/content/steinersp:QKP.png" alt="subir imagenes" border="0"></center>

<p></p><p>
Recall that a knight moves to any unoccupied square that is on the opposite corner of a 2x3 rectangle
from its current position; a queen moves to any square that is visible in any of the eight horizontal,
vertical, and diagonal directions from the current position. Note that the movement of a queen can be
blocked by another piece, while a knight¡¯s movement can not.

</p><h3>Input</h3>
<p>
There will be multiple test cases. Each test case will consist of 4 lines. The first line will contain
two integers n and m, indicating the dimensions of the board, giving rows and columns, respectively.
Neither integer will exceed 1000. The next three lines will each be of the form

</p><p></p><p>
<i>k r<sub>1</sub> c<sub>1</sub> r<sub>2</sub> c<sub>2</sub> ¡¤ ¡¤ ¡¤ r<sub>k</sub> c<sub>k</sub></i>

</p><p></p><p>
indicating the location of the queens, knights and pawns, respectively. The numbering of the rows and
columns will start at one. There will be no more than 100 of any one piece. Values of n = m = 0
indicate end of input.

</p><h3>Output</h3>
<p>
Each test case should generate one line of the form

</p><p></p><p>
<b><i>Board b has s safe squares.</i></b>

</p><p></p><p>
where <i>b</i> is the number of the board (starting at one) and you supply the correct value for <i>s</i>.

</p><h3>Example</h3>

<pre>4 4
2 1 4 2 4
1 1 2
1 2 3
2 3
1 1 2
1 1 1
0
1000 1000
1 3 3
0
0
0 0

<b>Output:</b>
Board 1 has 6 safe squares.
Board 2 has 0 safe squares.
Board 3 has 996998 safe squares.
</pre>