## 题目描述
You are given an unrooted weighted tree $T$ with vertices $1, 2, \ldots, n$. Please answer some queries.

We define $\texttt{dist}(i,j)$ as the distance between vertex $i$ and vertex $j$ in $T$.

For each query, you are given two integers $l, r$. Please answer the value of 

$$\min_{l\le i< j\le r}(\texttt{dist}(i,j)).$$

## 输入格式
The first line contains one integer $n~(1\leq n\le 2 \times 10^5)$, the number of vertices in the tree. 

Each of the next $n-1$ lines describes an edge of the tree. Edge $i$ is denoted by three integers $a_i, b_i, w_i$ $(1\le a_i, b_i\le n, 1\le w_i\le 10^9)$, the labels of vertices it connects and its weight. 

Then one line contains one integer $q~(1\leq q\le 10^6)$, the number of queries.

Each of the following $q$ lines contains two integers $l, r~(1\le l \le r\le n)$ describing a query.

It is guaranteed that the given edges form a tree.

## 输出格式

For each query, output the answer in one line. If there is no $i,j$ such that $l\le i<j\le r$, the answer is $-1$.

## 题目大意
给你一棵 $n$ 个点的树。记 $\operatorname{dist}(i,j)$ 为树上 $i,j$ 之间唯一简单路径的长度。

你要回答 $q$ 次询问：给定 $l,r$，求 $\min\limits_{l\leq i<j\leq r}(\operatorname{dist}(i,j))$。

```input1
5
1 2 5
1 3 3
1 4 4
3 5 2
5
1 1
1 4
2 4
3 4
2 5

```

```output1
-1
3
7
7
2

```

