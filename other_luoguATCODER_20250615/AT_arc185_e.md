# AT_arc185_e [ARC185E] Adjacent GCD

## 题目描述

定义一个整数序列 $B=(B_1,B_2,\dots,B_k)$ 的分数为 $\sum_{i=1}^{k-1}\gcd(B_i,B_{i+1})$。

给出一个整数序列 $A=(A_1,A_2,\dots,A_N)$，求出以下问题在 $m=1,2,\dots,N$ 时的答案：

- 序列 $A=(A_1,A_2,\dots,A_m)$ 有 $2^m-1$ 个非空子序列。求出这些子序列的分数之和对 $998244353$ 取模后的值。如果两个子序列在原序列中的位置不同，即使它们的元素全部相同，我们也认为它们是不同的。

## 输入格式

输入来自标准输入，格式如下：

> $N$
> $A_1\ A_2\ \dots\ A_N$

## 输出格式

输出 $N$ 行，第 $i$ 行表示当 $m=i$ 时的答案。

### 样例 1 解释

以 $m=3$ 为例。以下是 $(A_1,A_2,A_3)=(9,6,4)$ 的所有非空子序列和分数：

- $(9)$，分数为 $0$。  
- $(6)$，分数为 $0$。  
- $(4)$，分数为 $0$。  
- $(9,6)$，分数为 $\gcd(9,6)=3$。  
- $(9,4)$，分数为 $\gcd(9,4)=1$。
- $(6,4)$，分数为 $\gcd(6,4)=2$。
- $(9,6,4)$，分数为 $\gcd(9,6)+\gcd(6,4)=3+2=5$。

因此当 $m=3$ 时答案为 $0+0+0+3+1+2+5=11$。

## 输入输出样例 #1

### 输入 #1

```
3
9 6 4
```

### 输出 #1

```
0
3
11
```

## 输入输出样例 #2

### 输入 #2

```
5
3 8 12 6 9
```

### 输出 #2

```
0
1
13
57
155
```

## 输入输出样例 #3

### 输入 #3

```
10
47718 21994 74148 76721 98917 73766 29598 59035 69293 29127
```

### 输出 #3

```
0
2
14
35
97
372
866
1859
4273
43287
```

## 说明/提示

- $1\le N\le 5\times 10^5$
- $1\le A_i\le 10^5$
- 输入的值全部为整数