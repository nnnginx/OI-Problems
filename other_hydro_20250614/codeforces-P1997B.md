## Description

<div><p>There is a grid, consisting of $2$ rows and $n$ columns. Each cell of the grid is either free or blocked.</p><p>A free cell $y$ is reachable from a free cell $x$ if at least one of these conditions holds: </p><ul> <li> $x$ and $y$ share a side; </li><li> there exists a free cell $z$ such that $z$ is reachable from $x$ and $y$ is reachable from $z$. </li></ul><p>A connected region is a set of free cells of the grid such that all cells in it are reachable from one another, but adding any other free cell to the set violates this rule.</p><p>For example, consider the following layout, where white cells are free, and dark grey cells are blocked:</p><center> <img class="tex-graphics" src="./34835/file/lBv5Dt3u.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <p>There are $3$ regions in it, denoted with red, green and blue color respectively:</p><center> <img class="tex-graphics" src="./34835/file/PDH0Qw1Q.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> <p>The given grid contains at most $1$ connected region. Your task is to calculate the number of free cells meeting the following constraint:</p><ul> <li> if this cell is blocked, the number of connected regions becomes exactly $3$. </li></ul></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of columns.</p><p>The $i$-th of the next two lines contains a description of the $i$-th row of the grid&nbsp;！ the string $s_i$, consisting of $n$ characters. Each character is either <span class="tex-font-style-tt">.</span> (denoting a free cell) or <span class="tex-font-style-tt">x</span> (denoting a blocked cell). </p><p>Additional constraint on the input: </p><ul> <li> the given grid contains at most $1$ connected region; </li><li> the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$. </li></ul></div><div class="output-specification"><p>For each test case, print a single integer&nbsp;！ the number of cells such that the number of connected regions becomes $3$ if this cell is blocked.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases.</p><p>The first line of each test case contains a single integer $n$ ($1 \le n \le 2 \cdot 10^5$)&nbsp;！ the number of columns.</p><p>The $i$-th of the next two lines contains a description of the $i$-th row of the grid&nbsp;！ the string $s_i$, consisting of $n$ characters. Each character is either <span class="tex-font-style-tt">.</span> (denoting a free cell) or <span class="tex-font-style-tt">x</span> (denoting a blocked cell). </p><p>Additional constraint on the input: </p><ul> <li> the given grid contains at most $1$ connected region; </li><li> the sum of $n$ over all test cases doesn't exceed $2 \cdot 10^5$. </li></ul>

## Output

<p>For each test case, print a single integer&nbsp;！ the number of cells such that the number of connected regions becomes $3$ if this cell is blocked.</p>





```input1|2,3,4,8,9,10
4
8
.......x
.x.xx...
2
..
..
3
xxx
xxx
9
..x.x.x.x
x.......x
```




```output1
1
0
0
2
```



## Note

<p>In the first test case, if the cell $(1, 3)$ is blocked, the number of connected regions becomes $3$ (as shown in the picture from the statement).</p>
