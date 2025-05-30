<p>In the game of tic-tac-toe, two players take turns marking squares of an initially empty 3 �� 3 grid with either X��s or O��s. The first player always marks squares using X��s, whereas the second player always marks squares using O��s. If at any point during the game either player manages to mark three consecutive squares in a row, column, or diagonal with his/her symbol, the game terminates.

</p><p><br>
Given a board configuration, your goal is to determine whether the board configuration represents the possible final state of a valid tic-tac-toe game.

</p><p><br>
</p><h3>Input</h3>
<p>The input test file will contain multiple cases. Each test case consists of a single line containing 9 characters, which represent the 9 squares of a tic-tac-toe grid, given one row at a time. Each character on the line will either be ��X��, ��O�� (the letter O), or ��.�� (indicating an unfilled square). The end-of-file is marked by a single line containing the word ��end��.

</p><p><br>
</p><h3>Output</h3>
<p>For each input test case, write a single line containing either the word ��valid�� or ��invalid�� indicating whether the given board configuration is the final state of some possible tic-tac-toe game.

</p><p><br>
</p><h3>Example</h3>

<pre><b>Input:</b>
XXXOO.XXX
XOXOXOXOX
OXOXOXOXO
XXOOOXXOX
XO.OX...X
.XXX.XOOO
OOXXXOOXO
end

<b>Output:</b>
invalid
valid
invalid
valid
valid
invalid
invalid
</pre>