## Description

<div><p>There is a rectangular grid of size $n \times m$. Each cell of the grid is colored black ('<span class="tex-font-style-tt">0</span>') or white ('<span class="tex-font-style-tt">1</span>'). The color of the cell $(i, j)$ is $c_{i, j}$. You are also given a map of directions: for each cell, there is a direction $s_{i, j}$ which is one of the four characters '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>' and '<span class="tex-font-style-tt">L</span>'.</p><ul> <li> If $s_{i, j}$ is '<span class="tex-font-style-tt">U</span>' then there is a transition from the cell $(i, j)$ to the cell $(i - 1, j)$; </li><li> if $s_{i, j}$ is '<span class="tex-font-style-tt">R</span>' then there is a transition from the cell $(i, j)$ to the cell $(i, j + 1)$; </li><li> if $s_{i, j}$ is '<span class="tex-font-style-tt">D</span>' then there is a transition from the cell $(i, j)$ to the cell $(i + 1, j)$; </li><li> if $s_{i, j}$ is '<span class="tex-font-style-tt">L</span>' then there is a transition from the cell $(i, j)$ to the cell $(i, j - 1)$. </li></ul><p>It is guaranteed that the top row doesn't contain characters '<span class="tex-font-style-tt">U</span>', the bottom row doesn't contain characters '<span class="tex-font-style-tt">D</span>', the leftmost column doesn't contain characters '<span class="tex-font-style-tt">L</span>' and the rightmost column doesn't contain characters '<span class="tex-font-style-tt">R</span>'.</p><p>You want to place some robots in this field (at most one robot in a cell). The following conditions should be satisfied.</p><ul> <li> Firstly, each robot <span class="tex-font-style-bf">should move</span> every time (i.e. it cannot skip the move). <span class="tex-font-style-bf">During one move each robot goes to the adjacent cell depending on the current direction</span>. </li><li> Secondly, you have to place robots in such a way that <span class="tex-font-style-bf">there is no move</span> before which two different robots occupy the same cell (it also means that you cannot place two robots in the same cell). I.e. if the grid is "<span class="tex-font-style-tt">RL</span>" (one row, two columns, colors does not matter there) then you can place two robots in cells $(1, 1)$ and $(1, 2)$, but if the grid is "<span class="tex-font-style-tt">RLL</span>" then you cannot place robots in cells $(1, 1)$ and $(1, 3)$ because during the first second both robots will occupy the cell $(1, 2)$. </li></ul><p>The robots make an infinite number of moves.</p><p>Your task is to place the maximum number of robots to satisfy all the conditions described above and among all such ways, you have to choose one where the number of <span class="tex-font-style-bf">black</span> cells occupied by robots <span class="tex-font-style-bf">before all movements</span> is the maximum possible. <span class="tex-font-style-bf">Note that you can place robots only before all movements</span>.</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 5 \cdot 10^4$) ！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $m$ ($1 &lt; nm \le 10^6$) ！ the number of rows and the number of columns correspondingly.</p><p>The next $n$ lines contain $m$ characters each, where the $j$-th character of the $i$-th line is $c_{i, j}$ ($c_{i, j}$ is either '<span class="tex-font-style-tt">0</span>' if the cell $(i, j)$ is black or '<span class="tex-font-style-tt">1</span>' if the cell $(i, j)$ is white).</p><p>The next $n$ lines also contain $m$ characters each, where the $j$-th character of the $i$-th line is $s_{i, j}$ ($s_{i, j}$ is '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>' or '<span class="tex-font-style-tt">L</span>' and describes the direction of the cell $(i, j)$).</p><p>It is guaranteed that the sum of the sizes of fields does not exceed $10^6$ ($\sum nm \le 10^6$).</p></div><div class="output-specification"><p>For each test case, print two integers ！ the maximum number of robots you can place to satisfy all the conditions described in the problem statement and the maximum number of <span class="tex-font-style-bf">black</span> cells occupied by robots <span class="tex-font-style-bf">before all movements</span> if the number of robots placed is maximized. <span class="tex-font-style-bf">Note that you can place robots only before all movements</span>.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 5 \cdot 10^4$) ！ the number of test cases. Then $t$ test cases follow.</p><p>The first line of the test case contains two integers $n$ and $m$ ($1 &lt; nm \le 10^6$) ！ the number of rows and the number of columns correspondingly.</p><p>The next $n$ lines contain $m$ characters each, where the $j$-th character of the $i$-th line is $c_{i, j}$ ($c_{i, j}$ is either '<span class="tex-font-style-tt">0</span>' if the cell $(i, j)$ is black or '<span class="tex-font-style-tt">1</span>' if the cell $(i, j)$ is white).</p><p>The next $n$ lines also contain $m$ characters each, where the $j$-th character of the $i$-th line is $s_{i, j}$ ($s_{i, j}$ is '<span class="tex-font-style-tt">U</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">D</span>' or '<span class="tex-font-style-tt">L</span>' and describes the direction of the cell $(i, j)$).</p><p>It is guaranteed that the sum of the sizes of fields does not exceed $10^6$ ($\sum nm \le 10^6$).</p>

## Output

<p>For each test case, print two integers ！ the maximum number of robots you can place to satisfy all the conditions described in the problem statement and the maximum number of <span class="tex-font-style-bf">black</span> cells occupied by robots <span class="tex-font-style-bf">before all movements</span> if the number of robots placed is maximized. <span class="tex-font-style-bf">Note that you can place robots only before all movements</span>.</p>

## Samples

```input1
3
1 2
01
RL
3 3
001
101
110
RLL
DLD
ULL
3 3
000
000
000
RRD
RLD
ULL
```

```output1
2 1
4 3
2 2
```



