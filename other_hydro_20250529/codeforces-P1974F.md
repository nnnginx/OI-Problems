## Description

<div><p>Alice and Bob were playing a game again. They have a grid of size $a \times b$ ($1 \le a, b \le 10^9$), on which there are $n$ chips, with at most one chip in each cell. The cell at the intersection of the $x$-th row and the $y$-th column has coordinates $(x, y)$.</p><p>Alice made the first move, and the players took turns. On each move, a player could cut several (but not all) rows or columns from the beginning or end of the remaining grid and earn a point for each chip that was on the cut part of the grid. Each move can be described by the character '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">D</span>', '<span class="tex-font-style-tt">L</span>', or '<span class="tex-font-style-tt">R</span>' and an integer $k$:</p><ul> <li> If the character is '<span class="tex-font-style-tt">U</span>', then the first $k$ remaining rows will be cut; </li><li> If the character is '<span class="tex-font-style-tt">D</span>', then the last $k$ remaining rows will be cut; </li><li> If the character is '<span class="tex-font-style-tt">L</span>', then the first $k$ remaining columns will be cut; </li><li> If the character is '<span class="tex-font-style-tt">R</span>', then the last $k$ remaining columns will be cut. </li></ul><p>Based on the initial state of the grid and the players' moves, determine the number of points earned by Alice and Bob, respectively.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains four integers $a$, $b$, $n$, and $m$ ($2 \le a, b \le 10^9$, $1 \le n, m \le 2 \cdot 10^5$)&nbsp;！ the dimensions of the grid, the number of chips, and the number of moves.</p><p>Each of the next $n$ lines contain two integers $x_i$ and $y_i$ ($1 \le x_i \le a$, $1 \le y_i \le b$)&nbsp;！ the coordinates of the chips. All pairs of coordinates are distinct.</p><p>Each of the next $m$ lines contain a character $c_j$ and an integer $k_j$&nbsp;！ the description of the $j$-th move. It is guaranteed that $k$ is <span class="tex-font-style-bf">less than</span> the number of rows/columns in the current grid. In other words, a player cannot cut the entire remaining grid on their move.</p><p>It is guaranteed that the sum of the values of $n$ across all test cases in the test does not exceed $2 \cdot 10^5$. It is guaranteed that the sum of the values of $m$ across all test cases in the test does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each test case, output two integers&nbsp;！ the number of points earned by Alice and Bob, respectively.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains four integers $a$, $b$, $n$, and $m$ ($2 \le a, b \le 10^9$, $1 \le n, m \le 2 \cdot 10^5$)&nbsp;！ the dimensions of the grid, the number of chips, and the number of moves.</p><p>Each of the next $n$ lines contain two integers $x_i$ and $y_i$ ($1 \le x_i \le a$, $1 \le y_i \le b$)&nbsp;！ the coordinates of the chips. All pairs of coordinates are distinct.</p><p>Each of the next $m$ lines contain a character $c_j$ and an integer $k_j$&nbsp;！ the description of the $j$-th move. It is guaranteed that $k$ is <span class="tex-font-style-bf">less than</span> the number of rows/columns in the current grid. In other words, a player cannot cut the entire remaining grid on their move.</p><p>It is guaranteed that the sum of the values of $n$ across all test cases in the test does not exceed $2 \cdot 10^5$. It is guaranteed that the sum of the values of $m$ across all test cases in the test does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each test case, output two integers&nbsp;！ the number of points earned by Alice and Bob, respectively.</p>





```input1|2,3,4,5,6,7,15,16,17,18,19,20,28,29,30,31
6
4 4 3 2
4 1
3 3
2 4
D 2
R 1
4 4 3 3
4 1
3 2
2 3
D 1
L 1
U 2
3 5 3 2
1 3
2 2
3 3
R 2
R 2
6 4 4 2
1 4
2 3
5 3
1 1
R 1
U 1
9 3 2 1
6 1
3 3
D 8
10 10 2 5
7 5
9 1
R 1
L 2
D 1
U 4
D 1
```




```output1
2 1
2 0
0 3
1 1
2 0
0 1
```



## Note

<p>Below is the game from the first example:</p><center> <img class="tex-graphics" src="./34673/file/8gOKvNXC.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>On her turn, Alice cut $2$ rows from the bottom and scored $2$ points, then Bob cut $1$ column from the right and scored one point. Note that if Bob had cut $1$ row from the bottom, he would have also scored $1$ point.</p>
