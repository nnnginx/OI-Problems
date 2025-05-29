<p>   </p>
<table class="problems" style="width: 100%;" border="0">
<tbody>
<tr class="navigation">
<td width="50%"><a href="/problems/MARBLE/en/">English</a></td>
<td width="50%"><a href="/problems/MARBLE/vn/">Vietnamese</a></td>
</tr>
</tbody>
</table>
<p></p>
<p>ktuan usually plays a marble game in a square table of NxN cells. The game proceeds as the following:</p>
<ul>
<li>Initially, ktuan puts K obstacles into K cells of the table.</li>
<li>After that, ktuan makes Q turns. At the i<sup>th</sup> turn, ktuan flicks D<sub>i</sub> marbles from the outside of the board into one of the 4 sides of the board. The size of each marble fits perfectly into one cell.&nbsp; The marble goes through the cells in the same row/column until it goes out of the board or it meets an obstacle or another marble. If there is an obstacle or another marble at the first position then the marble will not be placed on the board.</li>
<li>After each turn, ktuan records the total number of cells that the marbles in that turn passing through.</li>
</ul>
<p>Write a program that simulates the game and for each turn, print the total number of cells that the marbles in that turn passing through.</p>
<h3>Input</h3>
<ul>
<li>The first line contains three integers N, K, Q.</li>
<li>Each line in the next K lines contains a pair (u, v) representing the coordinates (row, column) of an obstacle.</li>
<li>Each line in the next Q lines contains 4 values c, D, u, v. The character c could be 'L', 'R', 'T', or 'B' depending on whether the marbles go from the left, right, top, or bottom of the board. (u, v) represents the initial coordinates of the marbles and it should be a boundary cell (corresponding to c). D is the number of marbles in the current turn.</li>
</ul>
<h3>Output</h3>
<ul>
<li>For each turn, print the total number of cells that the marbles passing through.</li>
</ul>
<h3>Example</h3>
<pre><strong>Input</strong> <br>5 1 3<br>3 3<br>L 2 3 1<br>T 1 1 1<br>B 5 5 5<br><br><strong>Output</strong><br>3<br>2<br>25</pre>
<h3>Output details</h3>
<ul>
<li>The first marble of the first turn will go through the two cells (3, 1) and (3, 2) before facing an obstacle at (3, 3).</li>
<li>The next marble of the first turn will go through the cell (3, 1) before facing another marble at (3, 2). Thus, the total number of cells passed through is 3.</li>
<li>The first marble of the second turn will pass through the two cells (1, 1) and (2, 1) before facing a marble at the cell (3, 1).</li>
<li>Each marble of the last turn will go out of the board as it doesn't tough obstacle or another marble. Thus, each marble will pass through 5 cells.</li>
</ul>
<h3>Constraints</h3>
<ul>
<li>N ¡Ü 50000, K ¡Ü 10, Q ¡Ü 100000</li>
<li>In 1/3 of the test cases, N and Q do not exceed 1000.</li>
</ul>
<p> </p>