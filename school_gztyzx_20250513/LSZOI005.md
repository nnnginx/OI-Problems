
## 题目背景

小明被比赛上的最后一道简单的 EX 题难住了，他对此十分不满，于是他找到了你，想让你解出这道题。

## 题目描述

给你 $4$ 个数 $n,a,b,x$，以如下方式生成一个序列：

$s_1=1$，对于 $2 \le i\le n$，$s_i=x\times(a+b \times s_{i-1}) \mod 10^9+7$。

你需要在这个序列 $s$ 上找到最优的 $l$ 和 $r$，使得 $[l,r]$ 之间的数按位与的结果 乘上 这段区间按位或的结果 的积最大。

## 输入格式

第一行，$n$

第二行，$a,b,x$

## 输出格式

一个数，答案。

## 样例 #1


```input1
8 76643 38883 38744
```
```output1
573682658410785889
```

## 提示

对于 $100\%$ 的数据，$1 \le n \le10^7$，$1 \le a,b,x \le 10^9$。

由于本题目是 EX 题，所以分值为 $50$ 分，且没有部分分。

