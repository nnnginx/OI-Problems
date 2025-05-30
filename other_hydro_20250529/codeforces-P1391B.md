## Description

<div><p>Consider a conveyor belt represented using a grid consisting of $n$ rows and $m$ columns. The cell in the $i$-th row from the top and the $j$-th column from the left is labelled $(i,j)$. </p><p>Every cell, except $(n,m)$, has a direction <span class="tex-font-style-tt">R</span> (Right) or <span class="tex-font-style-tt">D</span> (Down) assigned to it. If the cell $(i,j)$ is assigned direction <span class="tex-font-style-tt">R</span>, any luggage kept on that will move to the cell $(i,j+1)$. Similarly, if the cell $(i,j)$ is assigned direction <span class="tex-font-style-tt">D</span>, any luggage kept on that will move to the cell $(i+1,j)$. If at any moment, the luggage moves out of the grid, it is considered to be lost. </p><p>There is a counter at the cell $(n,m)$ from where all luggage is picked. A conveyor belt is called <span class="tex-font-style-bf">functional</span> if and only if any luggage reaches the counter regardless of which cell it is placed in initially. More formally, for every cell $(i,j)$, any luggage placed in this cell should eventually end up in the cell $(n,m)$. </p><p>This may not hold initially; you are, however, allowed to <span class="tex-font-style-bf">change</span> the directions of some cells to make the conveyor belt functional. Please determine the minimum amount of cells you have to change.</p><p>Please note that it is always possible to make any conveyor belt functional by changing the directions of some set of cells.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n, m$ ($1 \le n \le 100$, $1 \le m \le 100$) &nbsp;�� the number of rows and columns, respectively.</p><p>The following $n$ lines each contain $m$ characters. The $j$-th character in the $i$-th line, $a_{i,j}$ is the initial direction of the cell $(i, j)$. Please note that $a_{n,m}=$ <span class="tex-font-style-tt">C</span>.</p></div><div class="output-specification"><p>For each case, output in a new line the minimum number of cells that you have to change to make the conveyor belt functional. </p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10$). Description of the test cases follows.</p><p>The first line of each test case contains two integers $n, m$ ($1 \le n \le 100$, $1 \le m \le 100$) &nbsp;�� the number of rows and columns, respectively.</p><p>The following $n$ lines each contain $m$ characters. The $j$-th character in the $i$-th line, $a_{i,j}$ is the initial direction of the cell $(i, j)$. Please note that $a_{n,m}=$ <span class="tex-font-style-tt">C</span>.</p>

## Output

<p>For each case, output in a new line the minimum number of cells that you have to change to make the conveyor belt functional. </p>

## Samples

```input1
4
3 3
RRD
DDR
RRC
1 4
DDDC
6 9
RDDDDDRRR
RRDDRRDDD
RRDRDRRDR
DDDDRDDRR
DRRDRDDDR
DDRDRRDDC
1 1
C
```

```output1
1
3
9
0
```




## Note

<p>In the first case, just changing the direction of $(2,3)$ to <span class="tex-font-style-tt">D</span> is enough.</p><p>You can verify that the resulting belt is functional. For example, if we place any luggage at $(2,2)$, it first moves to $(3,2)$ and then to $(3,3)$. </p><p>In the second case, we have no option but to change the first $3$ cells from <span class="tex-font-style-tt">D</span> to <span class="tex-font-style-tt">R</span> making the grid equal to <span class="tex-font-style-tt">RRRC</span>.</p>
