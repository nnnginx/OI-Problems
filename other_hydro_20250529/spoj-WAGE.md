<p style="text-align: justify;">Danny has created a new civilization on a 2D grid. At the outset each grid location may be occupied by one of three life forms: Woods, Axe, or Grass. Each day, differing life forms occupying horizontally or vertically adjacent grid locations wage war. In each war, Woods always defeat Axe, Axe always defeat Grass, and Grass always defeat Woods. At the end of the day, the winner expands its territory to include the loser's grid position. The loser vacates the position.Determine the territory occupied by each life form after n days.</p>
<h3 style="text-align: justify;">Input</h3>
<p style="text-align: justify;">The first line of input contains t, the number of test cases. Each test case begins with three integers not greater than 100: r and c, the number of rows and columns in the grid, and n. The grid is represented by the r lines that follow, each with c characters. Each character in the grid is W, A, or G, indicating that it is occupied by Woods, Axe, or Grass respectively.</p>
<h3>Output</h3>
<p>For each test case, print the grid as it appears at the end of the nth day.</p>
<h3>Example</h3>
<pre><strong>Input:</strong><br>2 <br>3 3 1 <br>WWW <br>WAW <br>WWW <br>3 4 2 <br>WAGW <br>AGWA <br>GWAG</pre>
<pre><br><br><strong>Output:</strong>
WWW <br>WWW <br>WWW <br>&nbsp;<br>WWWA <br>WWAG <br>WAGW</pre>