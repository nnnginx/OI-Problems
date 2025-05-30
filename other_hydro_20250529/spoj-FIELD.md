<p>The Ministry of Defence (MoD) of Mighty Mouse Kingdom (MMK) needs to arrange defence forces in a battlefield to prevent possible attacks of Catland's army. The battlefield is a square grid of N rows and N columns. The cell in the i<sup>th</sup> row and j<sup>th</sup> column is denoted by (i,j), with 0 �� i, j �� N-1.</p>
<p>The MoD wants to put exactly N cannons in cells of the grid. Each cannon can guard all the cells that are in the same column or same row as it is. To minimize the cost, the MoD decides that each row and each column should be guarded by exactly one cannon.</p>
<p>Of course not all ways of arranging the cannons are equally good strategically. A cannon in cell (i, j) is said to be in a <em>safe</em> position if:</p>
<ul>
<li>1 �� j �� N-2</li>
<li>The row coordinates of the cannons in the j-1<sup>st</sup> and j+1<sup>st</sup> columns lie on the same side of the row coordinate i of the cannon (i,j). In other words, if we denote r<sub>k</sub> to be the row position of the cannon in the k<sup>th</sup> column, we should have either r<sub>j-1</sub> &lt; i and r<sub>j+1</sub> &lt; i, or r<sub>j-1</sub> &gt; i and r<sub>j+1</sub> &gt; i.
</li></ul>
<p>The Safety Index (SI) of the battlefield is the number of cannon in safe positions. Military strategists have pointed out that the SI must be at least K (K may vary depending on the weather, opponent's forces, etc.) in order to have a good defence of this important battlefield.</p>
<p>Compute the number of ways of arranging the cannons so that the SI is at least K.</p>
<h3>Input</h3>
<p>The first line contains t, the number of test cases (about 1000). Then t test cases follow. Each test case is described in a single line containing two numbers N and K (3 �� N �� 1000, 1 �� K �� N-2).</p>

<h3>Output</h3>
<p>For each test case, print a single line containing the number of ways of arranging the cannons so that the Safety Index is at least K. Since the result may be very large, you only need to print the remainder of the result when dividing by 30041975.</p>

<h3>Example</h3>

<pre><b>Input:</b>
3 
3 1
4 1
8 5

<b>Output:</b>
4
22
13102
</pre>

<h3>Output details</h3>
<p>Case 1: There are four ways of arranging the cannons: put the cannon at positions {(1,1), (2,3), (3,2)}, {(1,2), (2,3), (3,1)}, {(1,2), (2,1), (3,3)}, or {(1,3), (2,1), (3,1)}. The cannon in the middle column is always in the safe position.</p>