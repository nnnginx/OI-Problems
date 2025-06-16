<p>Petya and Vasya are inventing a new game that requires a rectangular board and one chess piece. At the beginning of the game the piece stands in the upper-left corner of the board. Two players move the piece in turns. Each turn the chess piece can be moved either one square to the right or one square down or jump <b><i>k</i></b> squares diagonally down and to the right. The player who can’t move the piece loses.
</p><p></p><center><img border="0" src="/content/shkoorah:cf36d.png"></center>
<p>The guys haven’t yet thought what to call the game or the best size of the board for it. Your task is to write a program that can determine the outcome of the game depending on the board size.

</p><h3>Input</h3>
<p>The first input line contains one integer 1  ≤  <b><i>t</i></b>  ≤  20202. Each of the following <b><i>t </i></b> lines contains three numbers:  <b><i>k</i></b> and <b><i>n</i></b>, <b><i>m</i></b> - the jump length and the board’s length and width (1  ≤ <b><i> n, m ,k</i></b> ≤  10<sup>9</sup>).

</p><h3>Output</h3>
<p>Output <b><i>t</i></b> lines that can determine the outcomes of the game on every board. Write «+» if the first player is a winner, and «-» otherwise.

</p><h3>Example</h3>

<pre><b>Input:</b>
10
1 1 1
1 2 1
2 1 2
2 2 2
1 3 2
2 3 2
3 1 3
3 2 3
3 3 3
4 3 3

<b>Output:</b>
-
+
+
-
+
+
-
+
-
-
</pre>