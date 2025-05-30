## 题目描述

我们称一个长度为 $2 \times n$ 的数列是有趣的，当且仅当该数列满足以下三个条件：

1. 它是从 $1$ 到 $2 \times n$ 共 $2 \times n$ 个整数的一个排列 $\{a_i\}$；
2. 所有的奇数项满足 $a_1<a_3< \dots <a_{2n-1}$，所有的偶数项满足 $a_2<a_4< \dots <a_{2 \times n}$；
3. 任意相邻的两项 $a_{2 \times i-1}$ 与 $a_{2 \times i}~(1 \leq i \leq n)$ 满足奇数项小于偶数项，即：$a_{2 \times i-1}<a_{2 \times i}$。

现在的任务是：对于给定的 $n$，请求出有多少个不同的长度为 $2 \times n$ 的有趣的数列。因为最后的答案可能很大，所以只要求输出答案 $\bmod P$的值。

## 输入格式

输入文件只包含用空格隔开的两个整数 $n$ 和 $P$。输入数据保证

输出格式
仅含一个整数，表示不同的长度为 2n 的有趣的数列个数 mod P 的值。

```input1
3 10
```

```output1
5
```

## 样例解释

对应的 $5$ 个有趣的数列分别为 $(1,2,3,4,5,6),(1,2,3,5,4,6),(1,3,2,4,5,6),(1,3,2,5,4,6),(1,4,2,5,3,6)$。

## 数据范围

$50\%$ 的数据满足 $n \leq 1000$

$100\%$ 的数据满足 $n \leq 10^6$ 且 $P \leq 10^9$。
