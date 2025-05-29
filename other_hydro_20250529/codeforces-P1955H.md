## Description

<div><p>You are playing a very popular Tower Defense game called "Runnerfield 2". In this game, the player sets up defensive towers that attack enemies moving from a certain starting point to the player's base.</p><p>You are given a grid of size $n \times m$, on which $k$ towers are already placed and a path is laid out through which enemies will move. The cell at the intersection of the $x$-th row and the $y$-th column is denoted as $(x, y)$.</p><p>Each second, a tower deals $p_i$ units of damage to all enemies within its range. For example, if an enemy is located at cell $(x, y)$ and a tower is at $(x_i, y_i)$ with a range of $r$, then the enemy will take damage of $p_i$ if $(x - x_i) ^ 2 + (y - y_i) ^ 2 \le r ^ 2$.</p><p>Enemies move from cell $(1, 1)$ to cell $(n, m)$, visiting each cell of the path exactly once. An enemy instantly moves to an adjacent cell horizontally or vertically, but before doing so, it spends one second in the current cell. If its health becomes zero or less during this second, the enemy can no longer move. The player loses if an enemy reaches cell $(n, m)$ and can make one more move.</p><p>By default, all towers have a zero range, but the player can set a tower's range to an integer $r$ ($r &gt; 0$), in which case the health of all enemies will increase by $3^r$. However, each $r$ can only be used for <span class="tex-font-style-bf">at most one</span> tower.</p><p>Suppose an enemy has a base health of $h$ units. If the tower ranges are $2$, $4$, and $5$, then the enemy's health at the start of the path will be $h + 3 ^ 2 + 3 ^ 4 + 3 ^ 5 = h + 9 + 81 + 243 = h + 333$. The choice of ranges is made once before the appearance of enemies and cannot be changed after the game starts.</p><p>Find the maximum amount of base health $h$ for which it is possible to set the ranges so that the player does not lose when an enemy with health $h$ passes through (without considering the additions for tower ranges).</p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \le t \le 100$) �� the number of test cases.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($2 \le n, m \le 50, 1 \le k &lt; n \cdot m$) �� the dimensions of the field and the number of towers on it.</p><p>The next $n$ lines each contain $m$ characters �� the description of each row of the field, where the character "." denotes an empty cell, and the character "#" denotes a path cell that the enemies will pass through.</p><p>Then follow $k$ lines �� the description of the towers. Each line of description contains three integers $x_i$, $y_i$, and $p_i$ ($1 \le x_i \le n, 1 \le y_i \le m, 1 \le p_i \le 500$) �� the coordinates of the tower and its attack parameter. All coordinates correspond to empty cells on the game field, and all pairs $(x_i, y_i)$ are pairwise distinct.</p><p>It is guaranteed that the sum of $n \cdot m$ does not exceed $2500$ for all test cases.</p></div><div class="output-specification"><p>For each test case, output the maximum amount of base health $h$ on a separate line, for which it is possible to set the ranges so that the player does not lose when an enemy with health $h$ passes through (without considering the additions for tower ranges).</p><p>If it is impossible to choose ranges even for an enemy with $1$ unit of base health, output "0".</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \le t \le 100$) �� the number of test cases.</p><p>The first line of each test case contains three integers $n$, $m$, and $k$ ($2 \le n, m \le 50, 1 \le k &lt; n \cdot m$) �� the dimensions of the field and the number of towers on it.</p><p>The next $n$ lines each contain $m$ characters �� the description of each row of the field, where the character "." denotes an empty cell, and the character "#" denotes a path cell that the enemies will pass through.</p><p>Then follow $k$ lines �� the description of the towers. Each line of description contains three integers $x_i$, $y_i$, and $p_i$ ($1 \le x_i \le n, 1 \le y_i \le m, 1 \le p_i \le 500$) �� the coordinates of the tower and its attack parameter. All coordinates correspond to empty cells on the game field, and all pairs $(x_i, y_i)$ are pairwise distinct.</p><p>It is guaranteed that the sum of $n \cdot m$ does not exceed $2500$ for all test cases.</p>

## Output

<p>For each test case, output the maximum amount of base health $h$ on a separate line, for which it is possible to set the ranges so that the player does not lose when an enemy with health $h$ passes through (without considering the additions for tower ranges).</p><p>If it is impossible to choose ranges even for an enemy with $1$ unit of base health, output "0".</p>





```input1|2,3,4,5,10,11,12,13,20,21,22,23,24,25
6
2 2 1
#.
##
1 2 1
2 2 1
#.
##
1 2 2
2 2 1
#.
##
1 2 500
3 3 2
#..
##.
.##
1 2 4
3 1 3
3 5 2
#.###
#.#.#
###.#
2 2 2
2 4 2
5 5 4
#....
#....
#....
#....
#####
3 2 142
4 5 9
2 5 79
1 3 50
```




```output1
0
1
1491
11
8
1797
```



## Note

<p>In the first example, there is no point in increasing the tower range, as it will not be able to deal enough damage to the monster even with $1$ unit of health.</p><p>In the second example, the tower has a range of $1$, and it deals damage to the monster in cells $(1, 1)$ and $(2, 2)$.</p><p>In the third example, the tower has a range of $2$, and it deals damage to the monster in all path cells. If the enemy's base health is $1491$, then after the addition for the tower range, its health will be $1491 + 3 ^ 2 = 1500$, which exactly equals the damage the tower will deal to it in three seconds.</p><p>In the fourth example, the tower at $(1, 2)$ has a range of $1$, and the tower at $(3, 1)$ has a range of $2$.</p>
