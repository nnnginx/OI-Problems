## 题目描述

Alice 和 Bob 在如上图的棋盘中移动一个同一个棋子，轮流行动，Alice 先手。每次可以上下左右移动，不能撞障碍，不能走已经走过的格子。不能行动的人就输了。对于每个起始位置，判断先手是否必胜。

## 输入格式

第一行输入两个整数 $n,m$。接下来是 $n$ 行 $m$ 列的矩阵，`.` 代表空地，`X` 代表障碍物。

一共有多组输入，以 `0 0` 结束。

## 输出格式

输出 $n$ 行 $m$ 列，`X` 代表障碍，`A` 代表先手必胜，`B` 代表先手必败。

```input1
1 1
.
3 3
...
.X.
...
1 4
....
3 3
X.X
...
X.X
5 8
........
.XX.XXX.
.X..X...
.X.XX.X.
........
0 0
```

```output1
B

AAA
AXA
AAA

AAAA

XBX
BAB
XBX

BABABABA
AXXBXXXB
BXBAXABA
AXAXXBXB
BABABABA
```

## 数据规模与约定

对于 $100\%$ 的数据，$0\le n,m\le 100$。

## 提示

对于最后一组样例：


![pic1](https://hydro.org.cn/d/bzoj/p/3078/file/pic1.jpg)

