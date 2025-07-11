# AT_arc148_e [ARC148E] ≥ K

## 题目描述

给定长度为 $n$ 的数列 $\{a_i\}$ 和一个自然数 $K$, 可以将 $\{a_i\}$ 打乱顺序重排，问多少种结果序列满足 $\forall i \in [1,n), a'_i + a'_{i+1} \ge K$。 答案对 $998244353$ 取模。

## 输入格式

$n\ \ K$    
$a_1\ \ a_2\ ... \ a_n$

## 输出格式

一个整数，答案对 $998244353$ 取模的结果。
##### 样例解释1
共 $4$ 个：$ (1,\ 4,\ 2,\ 3) - (1,\ 4,\ 3,\ 2)- (2,\ 3,\ 4,\ 1) - (3,\ 2,\ 4,\ 1)$

## 输入输出样例 #1

### 输入 #1

```
4 5
1 2 3 4
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
4 3
1 2 3 3
```

### 输出 #2

```
12
```

## 输入输出样例 #3

### 输入 #3

```
10 7
3 1 4 1 5 9 2 6 5 3
```

### 输出 #3

```
108
```

## 说明/提示

$ 2 \le n \le 2 \times 10^5$  
$ 0 \le a_i, K \le 10^9$