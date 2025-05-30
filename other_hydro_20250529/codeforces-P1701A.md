## Description

<div><p>There is a field of size $2 \times 2$. Each cell of this field can either contain grass or be empty. The value $a_{i, j}$ is $1$ if the cell $(i, j)$ contains grass, or $0$ otherwise.</p><p>In one move, you can choose <span class="tex-font-style-bf">one row</span> and <span class="tex-font-style-bf">one column</span> and cut all the grass in this row and this column. In other words, you choose the row $x$ and the column $y$, then you cut the grass in all cells $a_{x, i}$ and all cells $a_{i, y}$ for all $i$ from $1$ to $2$. After you cut the grass from a cell, it becomes empty (i. e. its value is replaced by $0$).</p><p>Your task is to find the minimum number of moves required to cut the grass in all non-empty cells of the field (i. e. make all $a_{i, j}$ zeros).</p><p>You have to answer $t$ independent test cases.</p></div><div class="input-specification"><p>The first line of the input contains one integer $t$ ($1 \le t \le 16$) — the number of test cases. Then $t$ test cases follow.</p><p>The test case consists of two lines, each of these lines contains two integers. The $j$-th integer in the $i$-th row is $a_{i, j}$. If $a_{i, j} = 0$ then the cell $(i, j)$ is empty, and if $a_{i, j} = 1$ the cell $(i, j)$ contains grass.</p></div><div class="output-specification"><p>For each test case, print one integer — the minimum number of moves required to cut the grass in all non-empty cells of the field (i. e. make all $a_{i, j}$ zeros) in the corresponding test case.</p></div>

## Input

<p>The first line of the input contains one integer $t$ ($1 \le t \le 16$) — the number of test cases. Then $t$ test cases follow.</p><p>The test case consists of two lines, each of these lines contains two integers. The $j$-th integer in the $i$-th row is $a_{i, j}$. If $a_{i, j} = 0$ then the cell $(i, j)$ is empty, and if $a_{i, j} = 1$ the cell $(i, j)$ contains grass.</p>

## Output

<p>For each test case, print one integer — the minimum number of moves required to cut the grass in all non-empty cells of the field (i. e. make all $a_{i, j}$ zeros) in the corresponding test case.</p>

## Samples

```input1
3
0 0
0 0
1 0
0 1
1 1
1 1
```

```output1
0
1
2
```



