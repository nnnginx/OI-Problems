## 题目描述

给长度为 $n$，值域在 $[1,inf]\cap\mathbb N$ 的数列 $a$。

$m$ 次询问 $l,r$，问区间有没有数的出现次数超过 $\lfloor\dfrac {r-l+1} {2} \rfloor$

## 输入格式

第一行两个整数 $n,inf$，如题所示。

接下来一行 $n$ 个整数，表示序列 $a$。

接下来一行一个整数 $m$。

接下来 $m$ 行，每行两个整数 $l,r$，描述一次询问。

## 输出格式

对每次询问，若存在答案，先输出 `yes`，再输出这个数。

否则输出 `no`。

## 提示说明

$1\le n\le 3\times 10^5,1\le m,inf\le10000$

## 题目来源

By Seter
