## 题目描述

在一个 $m$ 行 $n$ 列的棋盘里放一些彩色的棋子，使得每个格子最多放一个棋子，且不同颜色的棋子不能在同一行或者同一列，有多少种方法？例如，$n=m=3$，有两个白棋子和一个灰棋子，下面左边两种方法都是合法的，但右边两种都是非法的。

![](./2844/file/pic1.png) 

## 输入格式

输入第一行为两个整数 $n,m,c$，即行数、列数和棋子的颜色数。

第二行包含 $c$ 个正整数，即每个颜色的棋子数。

## 输出格式

输出仅一行，即方案总数除以 $10^9+9$ 的余数。

```input1
4 2 2
3 1
```

```output1
8
```

## 数据范围

对于所有数据，保证 $1\le n,m\le 30$，$1\le c\le 10$，总棋子数 $\le \max (250,n\times m)$。