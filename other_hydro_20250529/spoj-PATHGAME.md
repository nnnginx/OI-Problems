<p>Cat Snuke is playing the Path Game.</p>
<p>The Path Game is played on a rectangular grid of square cells. The grid has 2 rows and some positive number of columns. Each cell is either black or white.</p>
<p>A left-to-right path in the grid is a sequence of white cells such that the first cell in the sequence is in the leftmost column, the last cell in the sequence is in the rightmost column, and each pair of consecutive cells shares a common side.</p>
<p>The initial coloring of the grid is such that there is at least one left-to-right path. You are given this initial coloring as a 2D string. For each i and j, grid[i][j] is either '#' (representing a black cell) or '.' (representing a white cell).</p>
<p>Snuke may color some of the white cells black. After he does so, there must still be at least one left-to-right path left on the board. The goal of the game is to color as many cells black as possible. Compute and return the largest number of cells Snuke can color black. (Note that the cells that are already black do not count.)</p>
<h3>Input</h3>
<p>Input starts with an integer T (¡Ü 100), denoting the number of test cases.</p>
<p>Each case starts with an integer N (1 ¡Ü N ¡Ü 50), denoting the length of each row of the grid. Next two lines describe the 2D grid. Each line contains N characters ¡®.¡¯ or ¡®#¡¯. It is guaranteed that the grid will contain a left-right-right path.</p>
<h3>Output</h3>
<p>For each case, print one line containing the answer to the problem.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
2
5
#....
...#.
25
....#.##.....#...........
..#......#.......#..#....
</pre>
<pre><strong>Output:</strong>
2
13
</pre>