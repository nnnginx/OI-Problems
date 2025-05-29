## 题目描述

给一张地图，地图上有一些城市，城市之间可能有线路连通，我们用一个无向图来表示以简化概念，每条边有个权值，表示选择这条边需要花费的费用。给定 $4$ 对顶点（可能重复），求一个权值最小的边集，使得任意一对顶点可以由选出的边集中的边相连。

按照惯例，下面给出一个例子：

![](https://wenoide.gitee.io/bzoj/file/1866_0.jpg)

## 输入格式

第 $1$ 行 $2$ 个整数，$n$ 和 $m$，分别表示城市的个数和边的个数。

接下来 $n$ 行，每行一个字符串，表示每个城市的名字。城市的名字为一个不超过 $20$ 个字符，由小写字母构成的字符串。

再接下来 $m$ 行，每行给出 $s1$，$s2$ 和 $w$，其中 $s1$，$s2$ 为城市的名字，$w$ 为他们之间边的权值。

最后，给出 $4$ 行，每行给出两个字符串，分别为要求的一对城市的名字。

## 输出格式

一行，输出最小的花费。

## 样例

```input1
2 1
first
second
first second 10
first first
first first
second first
first first
```

```output1
10
```

```input2
10 15 stockholm amsterdam london berlin copenhagen oslo helsinki dublin reykjavik brussels oslo stockholm 415 stockholm helsinki 396 oslo london 1153 oslo copenhagen 485 stockholm copenhagen 522 copenhagen berlin 354 copenhagen amsterdam 622 helsinki berlin 1107 london amsterdam 356 berlin amsterdam 575 london dublin 463 reykjavik dublin 1498 reykjavik oslo 1748 london brussels 318 brussels amsterdam 173 stockholm amsterdam oslo london reykjavik dublin brussels helsinki
```

```output2
3907
```

## 数据规模与约定

对于 $10\%$ 或 $20\%$ 的数据，保证地图是一棵树。

对于所有数据，保证 $n\le 30,m\le 10^3,w\le 10^4$。

