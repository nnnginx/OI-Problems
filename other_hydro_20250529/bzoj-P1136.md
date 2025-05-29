## 题目描述

给定一个序列 $a_i$ 和一个整数 $k$ ，求出 $a$ 的一个长度为 $k$ 的子序列 $a_{bi}$ 满足：

1. $1 \le b_1 \le b_2 \le \dots \le b_k$。
2. 在满足 (1) 的情况下 $\{a_{b_1}, a_{b_2}, \dots , a_{b_k}\}$ 字典序最大。

## 输入格式

第一行一个数 $k$，以下一行，为序列 $a_i$。以一个单独的 $0$ 结束。

## 输出格式

$k$ 行，每行一个数，其中第 $i$ 行为 $a_{b_i}$。

```input1
12
5 8 3 15 8 0
```

```output1
12
15
8
```

## 数据规模与约定

$1 \le  a_i \le 10^9,k \le n \le 1.5 \times 10^7,k \le 10^6$.

## 提示

按照这里：http://main.edu.pl/en/archive/oi/16/arc 来写交互式的程序，然后把这个东西：http://oi.edu.pl/static/attachment/20110704/oi16-etap2-arc.zip 解压后把 `etap2/arc/prog` 里的 `carclib.c` 的内容贴到自己的源码中的一大堆“include”之前。这样这个程序就从交互式 程序变成普通的程序了，就可以AC了。

鸣谢 vfleaking。

