# AT_arc160_d [ARC160D] Mahjong

## 题目描述

找到可以通过以下两种操作，使得长度为 $N$、元素之和为 $M$ 的数列 $A$ 全为 $0$ 的 $A$ 的个数，再取模 $998244353$。

1. 在 $A$ 中选一个元素，将其减去 $K$。
2. 在 $A$ 中选取长度为 $K$ 的子串，子串中每个元素减去 $1$。

## 输入格式

输入一行整数，分别代表 $N~M~K$。

## 输出格式

输出答案。

## 输入输出样例 #1

### 输入 #1

```
3 2 2
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
100 998244353 100
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
2000 545782618661124208 533
```

### 输出 #3

```
908877889
```

## 说明/提示

- $1\le K\le N\le2000$
- $1\le M\le10^{18}$