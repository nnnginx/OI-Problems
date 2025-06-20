# AT_abc401_c [ABC401C] K-bonacci

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc401/tasks/abc401_c

给定正整数 $N$ 和 $K$。我们按照以下方式定义长度为 $N+1$ 的数列 $A=(A_0,A_1,\ldots,A_N)$ 的每个元素值：

- 当 $0 \leq i < K$ 时，$A_i = 1$
- 当 $K \leq i$ 时，$A_i = A_{i-K} + A_{i-K+1} + \ldots + A_{i-1}$

请计算 $A_N$ 对 $10^9$ 取模后的结果。

## 输入格式

输入通过标准输入给出，格式如下：

> $N$ $K$

## 输出格式

输出答案。

## 输入输出样例 #1

### 输入 #1

```
4 2
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
10 20
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
1000000 500000
```

### 输出 #3

```
420890625
```

## 说明/提示

### 约束条件

- $1 \leq N, K \leq 10^6$
- 输入的所有数值均为整数

### 样例解释 1

$A_0 = A_1 = 1$，而 $A_2 = A_0 + A_1 = 2$，$A_3 = A_1 + A_2 = 3$，$A_4 = A_2 + A_3 = 5$。

### 样例解释 3

请注意需要输出 $A_N$ 对 $10^9$ 取模后的结果。

翻译由 DeepSeek V3 完成