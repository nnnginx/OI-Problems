## Description

<div><p> </p><center><table class="tex-tabular"><tbody><tr><td class="tex-tabular-text-align-center tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-size-small"><span class="tex-font-style-it">There are no mountains in Florida, and Florida Man cannot comprehend their existence. As such, he really needs your help with this one.</span></span></td></tr></tbody></table></center><p>In the wilderness lies a region of mountainous terrain represented as a rectangular grid with $n$ rows and $m$ columns. Each cell in the grid is identified by its position $(i, j)$, where $i$ is the row index and $j$ is the column index. The altitude of cell $(i, j)$ is denoted by $a_{i,j}$.</p><p>However, this region has been tampered with. A path consisting of $n + m - 1$ cells, starting from the top-left corner $(1, 1)$ and ending at the bottom-right corner $(n, m)$, has been cleared. For every cell $(i, j)$ along this path, the altitude $a_{i,j}$ has been set to $0$. The path moves strictly via downward ($\mathtt{D}$) or rightward ($\mathtt{R}$) steps.</p><p>To restore the terrain to its original state, it is known that the region possessed a magical property before it was tampered with: all rows and all columns shared the same sum of altitudes. More formally, there exists an integer $x$ such that $\sum_{j=1}^m a_{i, j} = x$ for all $1\le i\le n$, and $\sum_{i=1}^n a_{i, j} = x$ for all $1\le j\le m$.</p><p>Your task is to assign new altitudes to the cells on the path such that the above magical property is restored. It can be proven that a solution always exists. If there are multiple solutions that satisfy the property, any one of them may be provided.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n, m \leq 1000$)&nbsp;！ the number of rows and columns in the grid.</p><p>The second line of each test case contains a string $s$ of length $n+m-2$ ($s_i = \mathtt{D}$ or $s_i = \mathtt{R}$)&nbsp;！ the steps the path makes from $(1, 1)$ to $(n, m)$. The character $\mathtt{D}$ represents a downward step, and $\mathtt{R}$ represents a rightward step.</p><p>The $i$-th of the next $n$ lines each contain $m$ integers $a_{i,1}, a_{i, 2}, \ldots, a_{i,m}$ ($-10^6 \leq a_{i,j} \leq 10^6$)&nbsp;！ the altitude of each cell in the grid. It is guaranteed that if a cell $(i, j)$ lies on the path, then $a_{i,j} = 0$.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $10^6$. </p></div><div class="output-specification"><p>For each test case, output $n$ lines of $m$ integers representing the restored grid of altitudes $b_{i, j}$. The altitudes must satisfy $-10^{15} \leq b_{i,j} \leq 10^{15}$, and additionally $a_{i,j} = b_{i,j}$ if $(i, j)$ is not on the path. If multiple solutions exist, output any of them.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n$ and $m$ ($2 \leq n, m \leq 1000$)&nbsp;！ the number of rows and columns in the grid.</p><p>The second line of each test case contains a string $s$ of length $n+m-2$ ($s_i = \mathtt{D}$ or $s_i = \mathtt{R}$)&nbsp;！ the steps the path makes from $(1, 1)$ to $(n, m)$. The character $\mathtt{D}$ represents a downward step, and $\mathtt{R}$ represents a rightward step.</p><p>The $i$-th of the next $n$ lines each contain $m$ integers $a_{i,1}, a_{i, 2}, \ldots, a_{i,m}$ ($-10^6 \leq a_{i,j} \leq 10^6$)&nbsp;！ the altitude of each cell in the grid. It is guaranteed that if a cell $(i, j)$ lies on the path, then $a_{i,j} = 0$.</p><p>It is guaranteed that the sum of $n \cdot m$ over all test cases does not exceed $10^6$. </p>

## Output

<p>For each test case, output $n$ lines of $m$ integers representing the restored grid of altitudes $b_{i, j}$. The altitudes must satisfy $-10^{15} \leq b_{i,j} \leq 10^{15}$, and additionally $a_{i,j} = b_{i,j}$ if $(i, j)$ is not on the path. If multiple solutions exist, output any of them.</p>





```input1|2,3,4,5,6,13,14,15,16
4
3 3
DRRD
0 2 3
0 0 0
3 1 0
4 5
DRRRRDD
0 1 0 2 3
0 0 0 0 0
-1 0 -3 -3 0
0 0 0 -1 0
2 3
RRD
0 0 0
0 1 0
5 5
DDDDRRRR
0 25 2 9 11
0 6 13 20 22
0 17 24 1 8
0 3 10 12 19
0 0 0 0 0
```




```output1
1 2 3
2 3 1
3 1 2
-6 1 0 2 3
7 -1 3 2 -11
-1 0 -3 -3 7
0 0 0 -1 1
0 -1 1
0 1 -1
18 25 2 9 11
4 6 13 20 22
15 17 24 1 8
21 3 10 12 19
7 14 16 23 5
```



## Note

<p>In the first test case, the grid has been filled such that every row and column contains the numbers $1, 2, 3$ in some order, resulting in a common sum of $6$.</p><p>In the second test case, the grid has been filled such that all rows and columns sum to $0$.</p>
