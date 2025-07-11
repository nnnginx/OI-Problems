# AT_abc372_b [ABC372B] 3^A

## 题目描述

你会得到一个正整数 $M$。找到一个正整数 $N$ 和一个非负整数序列 $A=(A_1,A_2,\dots,A_n)$，并且满足以下限制：

- $1\le N\le 20$
- $0\le A_i\le 10(1\le i\le N)$
- $\sum\limits_{i=1}^{N}3^{A_i}=M$ 

可以被证明，总是存在一组满足条件的 $N$ 和序列 $A$。

## 输入格式

一个整数 $M$。

## 输出格式

第一行，一个整数 $N$。

第二行有 $N$ 个整数，表示序列 $A$。

如果存在多组满足条件的 $N$ 和序列 $A$，任意一个都会被视为是正确的。

### 样例 1 解释

在样例中，$N=2$，$A=(1,1)$，我们有 $\sum\limits_{i=1}^N3^{A_i}=3+3=6$，满足限制。

此外，当 $N=4$，$A=(0,0,1,0)$ 时也满足限制。 

### 样例 3 解释

注意 $1\le N\le 20$ 的限制。

## 输入输出样例 #1

### 输入 #1

```
6
```

### 输出 #1

```
2
1 1
```

## 输入输出样例 #2

### 输入 #2

```
100
```

### 输出 #2

```
4
2 0 2 4
```

## 输入输出样例 #3

### 输入 #3

```
59048
```

### 输出 #3

```
20
0 0 1 1 2 2 3 3 4 4 5 5 6 6 7 7 8 8 9 9
```

## 说明/提示

- $1\le M\le 10^5$