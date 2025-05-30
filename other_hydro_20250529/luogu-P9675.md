## 题目描述
You are given an undirected weighted graph $G$ with vertices $1, 2, \ldots, n$. Please output the sum of the answers to the following $x$ questions:
- The $i$-th question $(1\le i\le x$): What is the minimum length of path that starts at vertex $1$, ends at vertex $n$, and contains exactly $i$ edges?

For each question, if such a path does not exist, the answer is considered to be $0$. A path may use one edge multiple times. Output the answer modulo $998244353$. 


## 输入格式
The first line contains one integer $T~(1 \le T\le 2000)$, the number of test cases.

For each test case, the first line contains three integers $n, m, x~(1\le n\le 2000, 0\le m\le 5000, 1\le x\le 10^9)$. Each of the next $m$ lines describes an edge of the graph. Edge $i$ is denoted by three integers $a_i, b_i, w_i$ $(1\le a_i, b_i\le n, 1\le w_i\le 10^9)$, the labels of vertices it connects and its weight. Note that self-loops and parallel edges may exist.

It is guaranteed that the sum of $n$ over all test cases is no more than $2000$ and the sum of $m$ over all test cases is no more than $5000$.

## 输出格式
For each test case, output one integer modulo $998244353$ denoting the answer.

## 题目大意
### 题目描述

给定一张 $n$ 个点 $m$ 条边的无向图 $G$，边有边权。你要回答 $x$ 个问题，其中第 $i$ $(1\leqslant i\leqslant x)$ 个问题形如：

- 从结点 $1$ 出发，经过 **恰好** $i$ 条边，到达结点 $n$ 的最短路径长度为多少？

对于每个询问，若不存在这样的路径，答案应当为 $0$。一条路径可能 **多次** 经过一条边。

求出这 $x$ 个问题所对应的答案之和。输出答案对 $998244353$ 取模后的结果。

### 输入格式

第一行包含一个整数 $T$ $(1\leqslant T\leqslant 2000)$，表示测试数据组数。

对于每组测试数据：

第一行三个整数 $n,m,x$ $(1\leqslant n\leqslant 2000,0\leqslant m\leqslant 5000,1\leqslant x\leqslant 10^9)$。

接下来 $m$ 行，每行三个整数 $a_i,b_i,w_i$ $(1\leqslant a_i,b_i\leqslant n,1\leqslant w_i\leqslant 10^9)$，分别表示第 $i$ 条边连接的两个结点的编号和其边权。注意 **可能存在自环和重边**。

保证所有测试数据中 $n$ 的总和不超过 $2000$，且 $m$ 的总和不超过 $5000$。

### 输出格式

对于每组测试数据，输出这组测试数据对应的答案 $\bmod$ $998244353$ 后的结果。

```input1
4
3 2 10
1 2 5
2 3 4
3 0 1000000000
3 3 100
1 2 3
1 3 4
2 3 5
4 6 1000000000
1 2 244
1 2 325
1 4 927
3 3 248
2 4 834
3 4 285
```

```output1
125
0
15300
840659991
```

