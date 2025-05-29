<p>In a modification of the popular game 'Pacman', the player has to move in a two-dimensional grid. Several cells of the grid are blocked. The player can start from any cell that is not blocked and can move in any of the directions, i.e. north, west,south or east, provided that the cells are unblocked.<br><br>
As soon as the player passes a cell, an enemy is generated in that cell, making it impossible for the player to pass through that cell again. Thus, the player can pass through any given cell only once. The player has to traverse all the unblocked cells in the grid in order to win .<br><br>
The player can begin at any free cell. Note that the same path with different starting points and even with the same
starting point but with different paths of traversal is treated as different routes. The problem requires you to print the total number of all such possible routes.

</p><h3>Input</h3>
<p>Each test case starts with a line containing two integers, m and n. Each of the next m lines contain a string of n characters describing the configuration of the grid. '*' denotes a blocked cell and '.' denotes unblocked cells. The input ends with a case having m = 0 and n = 0 and this case need not be processed.

</p><h3>Output</h3>
<p>For each test case, print one line containing the total number of possible routes for the corresponding case. As this number can be quite large, you should print ans%1000000007 where ans is the required result.

</p><h3>Example</h3>

<pre><b>Input:</b>
3 3
...
.*.
...
3 7
...*...
.*.*.*.
.......
3 3
***
*.*
***
0 0


<b>Output:</b>
16
8
1
</pre>

<h3>Constraints and Limits</h3>
<p>m ¡Ü 100, n ¡Ü 7, number of test cases ¡Ü 50

</p>