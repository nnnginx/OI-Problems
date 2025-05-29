<p>Max2214 is a game that consists of a board of <strong>R</strong> rows and <strong>C</strong> columns and two kinds of blocks: Some of the blocks are 2 cells high and 2 cells wide, the others are 1 cell high and 4 cells wide.  Some of the cells of the board might be marked. The objective of the game is to place the most blocks on top of the board in a way that the blocks are aligned to the rows and columns, no pair of blocks overlap, marked cells do not contain any block, and the 1x4 blocks are placed horizontally exclusively. Also, blocks must be completely inside the board.</p>
<h3>Input</h3>
<p>The input consists in a single test case with a 15 seconds execution limit.</p>
<p>The test case begins with 2 integers <strong>R</strong> and <strong>C </strong>in a single line: (1 &lt;= <strong>R </strong>&lt;= 52) (1 &lt;=<strong> C</strong> &lt;= 22).</p>
<p>The next <strong>R</strong> lines contain <strong>C</strong> characters. Each character represents a cell. If a character is X, it means the cell is a marked cell. If the character is '.' (A dot character) it means the cell is not marked.</p>
<h3>Output</h3>
<p>Show a single line containing the maximum quantity of blocks that can be placed in the board following the rules mentioned above.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
<pre>4 5<br>X....<br>X..XX<br>X..XX<br>....X</pre>
<strong>Output:</strong> <br>
<pre>3</pre>
<br></pre>