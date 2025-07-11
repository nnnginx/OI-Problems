# AT_kupc2013_h N and K

## 题目描述

**【题目大意】**

在由 $1$ 到 $N$ 的整数组成的单调增加数列，考虑从数列的要素中取出任意 $2$ 个不同的数，不会被其他一方除尽。在这些数列中，取出的最大长度为 $L$，这样的数列 $(a_1,a_2,\ldots,a_L)$。对于每个答案，数列中的第 $k$ 小要素要求最小。但是，这样的数列 $(a_1,\ldots,a_L)$ 当存在多个时，输出作为 $a_K$ 值所能取得的最小值。

另外，当 $K>L$ 时，输出 $-1$。

## 输入格式

第一行一个数 $C$，后面 $2$ 到 $C+1$ 行每行两个数 $N_i,K_i$。

## 输出格式

输出共 $C$ 行，第 $i$ 行的输出是关于 $N_i$ 和 $K_i$ 的回答，对于第 $i$ 行的答案，数列中的第 $k$ 小要素要求最小。

**【样例解释】**

$N=3$ 时，作为第二小要素最小的组合的一个例子 $(2,3)$。

$N=5$ 时，作为第二小要素最小的组合的一例 $(2,3,5)$。

$N=8$ 时，作为第三小要素最小的组合的一个例子 $(3,4,5,7)$。

$N=10$ 时，作为第一小要素最小的组合的一个例子 $(4,6,7,9,10)$。

## 说明/提示

$1 \leq C \leq 10^5$，$1 \leq N_i \leq 10^{18}$，$1 \leq K_i \leq N_i$。