# AT_arc193_b [ARC193B] Broken Wheel

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc193/tasks/arc193_b

给定一个正整数 $N$ 和一个由 `0` 和 `1` 组成的长度为 $N$ 的字符串 $s_0s_1\ldots s_{N-1}$。

考虑由编号为 $0, 1, 2, \ldots, N$ 的 $(N+1)$ 个顶点和以下边构成的简单无向图 $G$：

- 对于每个 $i = 0, 1, \ldots, N-1$，顶点 $i$ 与顶点 $(i+1) \bmod N$ 之间有一条无向边。
- 对于每个 $i = 0, 1, \ldots, N-1$，当且仅当 $s_i = $ `1` 时，顶点 $i$ 与顶点 $N$ 之间有一条无向边。
- 除此之外没有其他边。

接下来，将 $G$ 的每条边任意定向以构造有向图 $G'$。即，对于 $G$ 中的每条无向边 $\{u, v\}$，将其替换为有向边 $(u, v)$ 或 $(v, u)$ 中的一种。

对于每个 $i = 0, 1, \ldots, N$，设 $G'$ 中顶点 $i$ 的入度为 $d_i$。求可能得到的序列 $(d_0, d_1, \ldots, d_N)$ 的数量对 $998244353$ 取模的结果。

## 输入格式

输入通过标准输入给出，格式如下：

> $N$ $s_0s_1\ldots s_{N-1}$

## 输出格式

输出答案。

## 输入输出样例 #1

### 输入 #1

```
3
010
```

### 输出 #1

```
14
```

## 输入输出样例 #2

### 输入 #2

```
20
00001100111010100101
```

### 输出 #2

```
261339902
```

## 说明/提示

### 约束条件

- $3 \leq N \leq 10^6$
- $N$ 是整数
- $s_i$ 是 `0` 或 `1`

### 样例解释 1

图 $G$ 包含以下 4 条无向边：$\{0, 1\}$、$\{0, 2\}$、$\{1, 2\}$、$\{1, 3\}$。例如，若将各边分别定向为 $0 \to 1$、$2 \to 0$、$2 \to 1$、$1 \to 3$，则得到的 $(d_0, d_1, d_2, d_3) = (1, 2, 0, 1)$。所有可能的 $(d_0, d_1, d_2, d_3)$ 共有 14 种，具体为：$(0, 1, 2, 1)$、$(0, 2, 1, 1)$、$(0, 2, 2, 0)$、$(0, 3, 1, 0)$、$(1, 0, 2, 1)$、$(1, 1, 1, 1)$、$(1, 1, 2, 0)$、$(1, 2, 0, 1)$、$(1, 2, 1, 0)$、$(1, 3, 0, 0)$、$(2, 0, 1, 1)$、$(2, 1, 0, 1)$、$(2, 1, 1, 0)$、$(2, 2, 0, 0)$。

翻译由 DeepSeek R1 完成