<h1>Description</h1>
<p><em>"Connect Four </em><em>is a two-player game in which the players first choose a color and then take turns dropping colored discs from the top into a seven-column, six-row grid. The pieces fall straight down, occupying the next available space within the column. The objective of the game is to connect four of one's own discs of the same color next to each other vertically, horizontally, or diagonally before his opponent."</em><em> �C Wikipedia.</em></p>
<p>Johnny plays with the connect-four board, Johnny has N discs and each disc has a number on it. Johnny drops these discs in the board columns. as Johnny was nervous he closed the top of the board and rotated it with different angles, when he rotate the board 90 degree, all pieces slide over their rows till they hit the board boundary or touch another piece. You will be given the board configuration and those rotation angles. And you should write a program that calculates the new discs�� positions.</p>
<h2>Input Format</h2>
<p>Input will start with <strong><em>T</em></strong> number of test cases. Followed by <strong><em>T</em></strong> test cases each test case starts with board dimensions <strong><em>R</em></strong> and <strong><em>C</em></strong> where <strong><em>R</em></strong> (1 &lt; <strong><em>R </em></strong>&lt; 100) is number of rows and <strong><em>C</em></strong> (1 &lt; <strong><em>C </em></strong>&lt; 100) is number of columns, and number of discs <strong><em>N </em></strong>(0 &lt;= <strong><em>N </em></strong>&lt;= <strong><em>R</em></strong>*<strong><em>C</em></strong>). Then <strong><em>N</em></strong> lines follow, each contains two integers: <strong><em>P</em></strong> specifying the column number (0 &lt;= <strong><em>P </em></strong>&lt; <strong><em>C</em></strong>) and <strong><em>Q </em></strong>specifying the disc number (0 &lt;= <strong><em>Q </em></strong>&lt;= 9). Then you will be given number of rotations <strong><em>L</em></strong> followed by <strong><em>L</em></strong> positive integers representing the rotation angles, all angles will be anti-clockwise in the main directions (90, 180, and 270) only.</p>
<h2>Output Format</h2>
<p>For each test case, output the result using the following format:</p>
<p><strong><em>k</em></strong> (the test case number starting at 1) followed by a period (on a line by itself), then the final configuration of the board. Each row on a line by itself, and each cell is either a "." (without quotes) if the cell is an empty or a number representing a piece.</p>
<p>&nbsp;</p>
<table border="1" cellspacing="0" cellpadding="0">
<tbody>
<tr>
<td width="284" valign="top">
<h2>Sample Input</h2>
</td>
<td width="284" valign="top">
<h2>Sample Output</h2>
</td>
</tr>
<tr>
<td width="284" valign="top">
<p>4</p>
<p>2 3</p>
<p>2</p>
<p>0 5</p>
<p>2 9</p>
<p>0</p>
<p>2 3</p>
<p>2</p>
<p>0 5</p>
<p>2 9</p>
<p>1 90</p>
<p>2 3</p>
<p>2</p>
<p>0 5</p>
<p>2 9</p>
<p>1 180</p>
<p>2 3</p>
<p>2</p>
<p>0 5</p>
<p>2 9</p>
<p>2 90 90</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
<p>&nbsp;</p>
</td>
<td width="284" valign="top">
<p>1.</p>
<p>...</p>
<p>5.9</p>
<p>2.</p>
<p>..</p>
<p>.9</p>
<p>.5</p>
<p>3.</p>
<p>...</p>
<p>9.5</p>
<p>4.</p>
<p>...</p>
<p>.95<strong></strong></p>
</td>
</tr>
</tbody>
</table>
<p>&nbsp;</p>