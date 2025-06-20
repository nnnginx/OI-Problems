# AT_abc150_f [ABC150F] Xor Shift

## 题目描述

给定两个长度为 $n$ 的序列 $a=\{a_0,a_1,\cdots,a_{n-1}\}$ 和 $b=\{b_0,b_1,\cdots,b_{n-1}\}$，输出所有有序数对 $(k,x)$ ，满足：  
1. $0\leq k<n$ 且 $x\geq 0$。
2. 序列 $a'=b$，其中 $a'_i = a_{i+k\bmod n}\operatorname{xor} x\ (0\leq i<n)$，“$\operatorname{xor}$”表示按位异或。

## 输入格式

第一行一个整数 $n$。  
第二行 $n$ 个整数，依次是 $a_0,a_1,\cdots,a_{n-1}$。  
第三行 $n$ 个整数，依次是 $b_0,b_1,\cdots,b_{n-1}$。

## 输出格式

输出所有满足条件有序对 $(k,x)$，每对占一行。如果没有满足条件的有序对，输出为空。

## 输入输出样例 #1

### 输入 #1

```
3
0 2 1
1 2 3
```

### 输出 #1

```
1 3
```

## 输入输出样例 #2

### 输入 #2

```
5
0 0 0 0 0
2 2 2 2 2
```

### 输出 #2

```
0 2
1 2
2 2
3 2
4 2
```

## 输入输出样例 #3

### 输入 #3

```
6
0 1 3 7 6 4
1 5 4 6 2 3
```

### 输出 #3

```
2 2
5 5
```

## 输入输出样例 #4

### 输入 #4

```
2
1 2
0 0
```

### 输出 #4

```

```

## 说明/提示

$1\leq n\leq 2\times 10^5$，$0\leq a_i,b_i<2^{30}$。