# AT_abc267_d [ABC267D] Index × A(Not Continuous ver.)

## 题目描述

有一个长度为 $N$ 整数数列 $A=(A_1,A_2,...,A_N)$ 。

现在假设有一个长度为 $M$ 的序列 $B$ ,并且 $B$ 是 $A$ 的**子序列**。请找到 $\sum_{i=1}^M i\times B_i$ 的最大值。

## 输入格式

输入按照下面的标准格式给出：

> $ N\ M \newline A_1 \ A_2 \ \dots\  A_N $

## 输出格式

一个整数，表示$\sum_{i=1}^M i\times B_i$ 的最大值。

## 输入输出样例 #1

### 输入 #1

```
4 2
5 4 -1 8
```

### 输出 #1

```
21
```

## 输入输出样例 #2

### 输入 #2

```
10 4
-3 1 -4 1 -5 9 -2 6 -5 3
```

### 输出 #2

```
54
```

## 说明/提示

#### 注意事项
若序列 $S$ 是长度为 $L$ 的数列 $T$ 的**子序列**，则 $S$ 是数列 $T$ 删除任意 $i\ (i\in [0,L])$ 个元素得到的。

比如说， $(10,30)$ 是 $(10,20,30)$ 的字串，但是 $(20,10)$ 不是。


+ $1\le M\le N\le 2000$
+ $-2\times 10^5\le A_i\le 2\times 10^5$
+ 所有输入数据均为整数

#### 样例解释
对于**样例一**，当 $B=(A_1,A_4)$ 时，$\sum_{i=1}^M i\times B_i=1\times 5+2\times 8=21$ 。因为不可能达到 $22$ 或者更大的值，所以答案是 $21$ 。