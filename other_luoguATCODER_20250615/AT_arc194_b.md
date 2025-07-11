# AT_arc194_b [ARC194B] Minimum Cost Sort

## 题目描述

给定一个排列 $P = (P_1, P_2, \ldots, P_N)$，它是 $(1, 2, \ldots, N)$ 的一个排列。高桥君可以对 $P$ 进行以下操作任意次（包括零次）：

- 选择一个满足 $1 \leq i \leq N-1$ 的整数 $i$。支付成本 $i$ 后，交换 $P_i$ 和 $P_{i+1}$ 的值。

请求出将 $P$ 按升序排序所需支付的最小总成本。

## 输入格式

输入通过标准输入给出，格式如下：

> $N$ $P_1$ $P_2$ $\ldots$ $P_N$

## 输出格式

输出将 $P$ 按升序排序所需的最小总成本。

## 输入输出样例 #1

### 输入 #1

```
3
3 2 1
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
5
2 4 1 3 5
```

### 输出 #2

```
6
```

## 输入输出样例 #3

### 输入 #3

```
2
1 2
```

### 输出 #3

```
0
```

## 说明/提示

### 约束条件

- $2 \leq N \leq 2 \times 10^5$
- $P$ 是 $(1, 2, \ldots, N)$ 的一个排列
- 输入均为整数

### 样例解释 1

高桥君可以按以下步骤排序 $P$：
- 支付成本 $1$，交换 $P_1=3$ 和 $P_2=2$，此时 $P = (2, 3, 1)$。
- 支付成本 $2$，交换 $P_2=3$ 和 $P_3=1$，此时 $P = (2, 1, 3)$。
- 支付成本 $1$，交换 $P_1=2$ 和 $P_2=1$，此时 $P = (1, 2, 3)$。

此时总成本为 $1 + 2 + 1 = 4$，这是可能的最小值。

翻译由 DeepSeek R1 完成