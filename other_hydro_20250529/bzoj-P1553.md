## 题目描述

计算给定范围内有多少种输入可以使输出为 $1$。

## 输入格式

第一行包含三个整数，分别表示输入的个数，门的个数，连接到输出的门的编号。以下的 $m$ 行描述网络中的连接情况。第 $i$ 行表示第 $i$ 个门的两个输入，两个输入为范围 $[-n,m]$ 之间的一个整数。如果输入是网络的第 $k$ 个输入，则连接的描述是一个整数 $-k$，如果输入是第 $j$ 个门，则连接的描述是一个整数 $j$。以下两行各有一个 $n$ 位二进制串，表示输入的上限和下限。
## 输出格式
包含一个整数，表示给定范围内有多少种输入可以使输出为 $1$。
## 样例输入
```
5 6 5
-1 -2
1 3
1 -2
2 -3
4 6
-4 -5
00111
01110
```
## 样例输出
```
5
```

## 数据范围
$3<n<100,3<m<3000$，而且网络中的门是用 $1$ 到 $m$ 之间的数任意编号的。
## 题目来源
HNOI2009 集训 Day7。


