<p>Theodore implements a new strategy game ¡°Defense of a Kingdom¡±. On each level a player defends the&nbsp;Kingdom that is represented by a rectangular grid of cells. The player builds crossbow towers in some&nbsp;cells of the grid. The tower defends all the cells in the same row and the same column. No two towers&nbsp;share a row or a column.</p>

<p>The penalty of the position is the number of cells in the largest undefended rectangle. For example, the&nbsp;position shown on the picture has penalty 12.</p>

<p><img title="Example position" src="../../../content/fidels:DEFKIN.png" alt="This position has a penalty of 12." width="658" height="239"></p>

<p>Help Theodore write a program that calculates the penalty of the given position.</p>

<h3>Input</h3>
<p>The first line of the input file contains the number of test cases.</p>
<p>Each test case consists of a line with three integer numbers: w ¡ª width of the grid, h ¡ª height of the&nbsp;grid and n ¡ª number of crossbow towers (1 ¡Ü w, h ¡Ü 40 000; 0 ¡Ü n ¡Ü min(w, h)).</p>
<p>Each of the following n lines contains two integer numbers x<sub>i</sub> and y<sub>i</sub> ¡ª the coordinates&nbsp;of the cell occupied by a tower (1 ¡Ü x<sub>i</sub> ¡Ü w; 1 ¡Ü y<sub>i</sub> ¡Ü h).</p>

<h3>Output</h3>
<p>For each test case, output a single integer number ¡ª the number of cells in the largest rectangle that is not defended by&nbsp;the towers.</p>

<h3>Example</h3>
<pre><strong>Input:</strong>
1
15 8 3
3 8
11 2
8 6

<strong>Output:</strong>
12</pre>