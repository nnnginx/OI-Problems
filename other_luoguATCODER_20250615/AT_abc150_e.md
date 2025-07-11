# AT_abc150_e [ABC150E] Change a Little Bit

## 题目描述

对于两个长度为 $n$ 的 $\texttt{01}$ 序列 $S,T$ ，我们定义 $f(S,T)$ 为通过以下操作将 $S$ 修改为 $T$ 的最小代价和: 选择一个 $S$ 中的二进制位 $S_{i}$ ，然后改变 $S_{i}$ 的 $\texttt{01}$ 状态，代价为 $D \times C_{i}$，其中 $D$ 是此次操作前满足 $S_{j}\ne T_{j}$ 的整数 $j$ 的数量，$C_{i}$ 是一个给定的序列中的一个值。

求当 $S$ 取 $2^n$ 种不同的状态，$T$ 取 $2^n$ 种不同的状态时，$f(S,T)$ 的和对 $1000000007$ 取模的结果。

## 输入格式

第一行一个整数 $n$

第二行 $n$ 个整数 $C_{i}$

## 输出格式

一行一个整数，表示答案

## 输入输出样例 #1

### 输入 #1

```
1
1000000000
```

### 输出 #1

```
999999993
```

## 输入输出样例 #2

### 输入 #2

```
2
5 8
```

### 输出 #2

```
124
```

## 输入输出样例 #3

### 输入 #3

```
5
52 67 72 25 79
```

### 输出 #3

```
269312
```

## 说明/提示

$1 \le n \le 200000 , 1 \le C_{i} \le 10^9 $