<p>Sheldon and Penny are neighbours. Penny really likes grid games so Sheldon develops a new grid based game for Penny. The game consists of a MXN grid (M rows, N columns) and an infinite number of black and white knights. The grid has some open and some closed blocks. In the beginning of the game each player chooses his colour of knight.The rule says that each player on his turn can place his knight on any of the open blocks such that none of his knights attack any knight of other colour (he may attack any knight of the same colour). You are given a MXN grid. Specify the maximum number of knights (black+white) which can be placed on the grid. The game stops when any one player cannot place any more knights.</p>
<p>Note: In one turn, Knight can move exactly two squares horizontally and one square vertically, or two squares vertically and one square horizontally.</p>
<h3>Input</h3>
<p>First line specifies T, the number of test cases.</p>
<p>First line of each test case gives M and N seperated by a single space</p>
<p>This is followed by a grid of size MXN consisting of ¡®.¡¯ And ¡®#¡¯. Each ¡®.¡¯ represents an open<br>position and each ¡®#¡¯ represents closed position.</p>
<h3>Output</h3>
<p>Output 1 line for each test case giving the maximum possible value of knights that can be placed.</p>
<h3>Constraints</h3>
<p>1&lt;=T&lt;=5<br>1&lt;=M,N&lt;=10<br>0&lt;= No. of open positions "." &lt;=10</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
3 3
...
...
...
3 3
...
.#.
...

<strong>Output:</strong>
7
6</pre>