# AT_abc186_d [ABC186D] Sum of difference

## 题目描述

### 题意简述
输入 $n$ 个整数 $a_1,a_2,...a_n$，

求在满足 $1 \leq i < j \leq n$ 的所有 $\lvert a_i-a_j \rvert$ 的和 $X$ 。

即求 $X=\sum_{i=1}^{n-1}\sum_{j=i+1}^{n} \lvert a_i-a_j\rvert$ 。

## 输入格式

第一行是一个整数 $n$；

第二行是 $n$ 个整数 $a_1,a_2,\dots,a_n$。

所有数据保证 $2 \leq n \leq 2\times 10^5,\lvert a_i\rvert \leq 10^8。$

## 输出格式

输出所求的 $X$。

## 输入输出样例 #1

### 输入 #1

```
3
5 1 2
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
5
31 41 59 26 53
```

### 输出 #2

```
176
```