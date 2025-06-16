## 题目描述

In an edge-weighted tree, the xor-length of a path $p$ is defined as the xor sum of the weights of edges on $p$:

$$_{xor}length(p)=\oplus_{e \in p}w(e)$$

$\oplus$ is the xor operator.

We say a path the xor-longest path if it has the largest xor-length. Given an edge-weighted tree with $n$ nodes, can you find the xor-longest path?

给定一棵 $n$ 个点的带权树，求树上最长的异或和路径。

## 输入格式

The input contains several test cases. The first line of each test case contains an integer $n$, The following $n-1$ lines each contains three integers $u, v, w$ ($0 \le u \lt n$, $0 \le v \lt n$), which means there is an edge between node $u$ and $v$ of length $w$.

## 输出格式

For each test case output the xor-length of the xor-longest path.

```input1
4
1 2 3
2 3 4
2 4 6
```
```output1
7
```

## 样例说明

The xor-longest path is $1 \to 2 \to 3$, which has length $7$ ($3 \oplus 4$).

## 提示

注意：结点下标从 $1$ 开始到 $n$。

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 10^5$，$0 \le w \lt 2^{31}$。

