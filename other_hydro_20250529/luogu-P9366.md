## 题目描述
Given a square grid, its lattice points labeled from $(0, 0)$ to $(n, n)$, and a number $t$.

You need to answer $q$ queries in this format: given $A = (x_0, y_0)$ and $B = (x_1, y_1)$, how many ways are there to move from $A$ to $B$ in exactly $t$ steps so that in each step you move from a lattice point to one of its neighbors (up, down, left, right). Calculate the answer modulo $998\,244\,353$.

## 输入格式
The first line contains three integers $n$ ($1 \leq n \leq 10^5$), $t$ ($1 \leq t \leq 10^9$) and $q$ ($1 \leq q \leq 3 \times 10^5$).

Each of the following $q$ lines contains four integers $x_0$, $y_0$, $x_1$ and $y_1$ ($0 \leq x_0, y_0, x_1, y_1 \leq n$), representing a query. 

## 输出格式
For each query, output a line containing one integer, representing the answer to the query modulo $998\,244\,353$.

## 题目大意
给定正方形网格，格点坐标从 $(0,0)$ 到 $(n,n)$。

$q$ 组询问，每次询问从 $(x_0, y_0)$ 走恰好 $t$ 步，每步只能朝上、下、左、右走一格，不走出边界，走到 $(x_1, y_1)$ 的方案数，对 $998\,244\,353$ 取模。所有询问的 $t$ 相同。

```input1
2 5 3
0 0 1 2
1 1 2 1
0 0 2 2

```

```output1
30
64
0

```

```input2
5 20 5
0 0 5 5
1 1 4 4
2 2 3 3
2 3 2 3
1 2 5 2

```

```output2
615136704
443203969
899931333
464755094
679729107

```

## 提示
**Source**: The 2022 ICPC Asia Xi'an Regional Contest Problem I.

**Author**: djq_cpp.

