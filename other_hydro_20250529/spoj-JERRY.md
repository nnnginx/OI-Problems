<p>Have you heard about Jerry from Tom &amp; Jerry cartoon, we all loved that when we were young. Jerry has been put into a grid of <em>n</em> by <em>n</em> cells, with only <em>k</em> cells containing cheese. The rest of the cells are empty. Now, Jerry can start his journey from any cell of the grid he wants and move from one cell to any of its four adjacent cells. That is he can move up, down, left, or right in one move. When he reaches a cell containing cheese he can eat that cheese. Otherwise, he will move to the next cell. If the initial cell that Jerry lands on has cheese in it, he can eat that too.</p>
<p>Unfortunately for Jerry, he can¡¯t plan his trip very well. He can only rely on his sense of smell. From any cell, he will choose the path to go to the closest cell with cheese. Here, we calculate the distance between any two cells using the definition of ¡°Manhattan Distance¡±. If there are multiple cells with cheese with the same distance, he chooses top most cell among the tied the cells. If even after this the tie is not broken (i.e. the tied cells are in the same row) then he chooses the leftmost cell.</p>
<p>Also, Jerry can not eat all <em>k</em> cheeses as he gets full after eating <em>c</em> cheeses. It is guaranteed that there are at least <em>c</em> cheese in the grid. After eating <em>c</em> cheeses his journey ends immediately and is taken out of the grid. As Jerry does not like to run around more than he has to, he wants to minimize the number of cells he needs to visit.</p>
<p>Now, as a friend of Jerry, your task is to figure out, which cell Jerry should start his journey, so that he has to move to least number of cells to eat c cheeses. You don¡¯t need to tell us about the starting cell though, only tell us the minimum moves required by Jerry to eat c cheeses.</p>
<p>Note that, the ¡°Manhattan Distance¡± between two points in a grid is based on a strictly horizontal and/or vertical path (that is, along the grid lines), as opposed to the diagonal or ¡°as the crow flies¡± distance. The Manhattan distance is the simple sum of the horizontal and vertical components, whereas the diagonal distance might be computed by applying the Pythagorean theorem.</p>
<h3>Input</h3>
<p>The first line contains an integer, <em>T</em>, denoting the number of test cases to follow. For each test case, the first line contains 3 space separated integers: <em>n</em>, <em>k</em>, and <em>c</em>. Next <em>n</em> lines represents the grid. Each of those <em>n</em> lines has <em>n</em> characters representing each cell. Each cell can is represented either by ¡®.¡¯ representing empty cell and ¡®*¡¯ representing cell with cheese.</p>
<h4>Constraints</h4>
<ul>
<li>T ¡Ü 100</li>
<li>1 ¡Ü n ¡Ü 100</li>
<li>1 ¡Ü k ¡Ü 1000</li>
<li>k ¡Ü n<sup>2</sup></li>
<li>1 ¡Ü c ¡Ü 10</li>
<li>c ¡Ü k</li>
</ul>
<h3>Output</h3>
<p>For each test case print the least number of moves Jerry has to make to eat <em>c</em> cheeses.</p>
<h3>Example</h3>
<pre><strong>Input:</strong>
3
3 2 1
..*
*..
...
3 3 2
*.*
.*.
...
6 6 4
*.*.*.
.*....
......
....*.
*.....
......
<strong>Output:</strong>
0
2
6
</pre>
<h3>Explanation</h3>
<p>For the first test case, we can drop Jerry to any of the two cells containing cheese so that he can immediately eat 1 cheese and does not have to move at all.</p>
<p>For the second test case, again we can drop Jerry on any of the cell with cheese. For example, Jerry can be dropped on the second cell of the second row from the top. Jerry eats cheese on this cell. There are two remaining cells with cheese, both of which are 2 moves away. However, Jerry will choose the the first cell on the first row to move next.</p>
<p>For the last test case, Jerry can be dropped on the second cell on the second row. From there, Jerry moves to the first cell on the first row and continue moving right until he eats 4 cheeses in total.</p>