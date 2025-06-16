# AT_abc281_e [ABC281E] Least Elements

## 题目描述

给定一个序列 $A$，对于每个 $1 \le i \le N - M + 1$，将 $A_i A_{i + 1} \cdots A_{i + M - 1}$ **从小到大**排序后（不影响原序列），求出 $\displaystyle ans_i = \sum\limits_{j=i}^{i+k-1} A_j$。

## 输入格式

> $N, M, K\\ A_1 A_2 \cdots A_N$

## 输出格式

> $\mathrm{ans}_1 \mathrm{ans}_2 \cdots \mathrm{ans}_{N-M+1}$

## 输入输出样例 #1

### 输入 #1

```
6 4 3
3 1 4 1 5 9
```

### 输出 #1

```
5 6 10
```

## 输入输出样例 #2

### 输入 #2

```
10 6 3
12 2 17 11 19 8 4 3 6 20
```

### 输出 #2

```
21 14 15 13 13
```

## 说明/提示

$1 \le K \le M \le N \le 2 \times 10^5$

$1 \le A_i \le 10^9$