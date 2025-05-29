<p>There is a checkmates board with <b>n</b> rows and <b>m</b> columns. Some of the cells of the board are occupied. There is a queen standing on a certain cell. It wants to move to another cell of this board. Help it do this making the least possible moves. The queen can go any number of cells in any of eight directions in a single move, but it can't pass through or stand on the occupied cells and leave the board.</p>

<h3>Input</h3>
<p>The first line of the input contains number <b>t</b> 每 the amount of tests. Then <b>t</b> test descriptions follow. The first line of each test consists of two numbers <b>n</b> and <b>m</b> separated with a space. Then <b>n</b> lines follow each containing <b>m</b> characters describing the board. Character ＆.＊ means a free cell, character ＆X＊ 每 an occupied cell, character ＆S＊ 每 the starting cell of the queen, character ＆F＊ 每 the cell where the queen wants to go. It is guaranteed that there will be exactly one character ＆S＊ and one character ＆F＊ on each board.</p>

<h3>Constraints</h3>
<p>1 &lt;= <b>t</b> &lt;= 30<br>
2 &lt;= <b>n</b>, <b>m</b> &lt;= 1000</p>

<h3>Output</h3>
<p>For each test case print the minimum number of moves the queen has to do to reach the desired cell. Print ＆-1＊ if the queen can＊t reach the cell.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3
3 3
S..
...
..F
3 3
S..
XX.
F..
3 3
S..
XXX
..F

<b>Output:</b>
1
3
-1
</pre>