## 题目描述

有一个装球机器，构造可以看作是一棵树。有下面两种操作：从根放入一个球，只要下方有空位，球会沿着树滚下。如果同时有多个点可以走，那么会选择编号最小的节点所在路径的方向。比如依次在树根 $4$ 放 $2$ 个球，第一个球会落到 $1$，第二个会落到 $3$：

![pic1.jpg](./2683/file/pic1.jpg)

从某个位置拿走一个球，那么它上方的球会落下来。比如依次拿走 $5, 7, 8$ 三个球：

![pic2.jpg](./2683/file/pic2.jpg)

## 输入格式

第一行两个整数 $n,q$。

下面 $n$ 行，每行一个整数，表示第 $i$ 个节点的父亲。如果是根，则为 $0$。

接下来 $Q$ 行，每行两个整数 $\rm op~num$

1. $\rm op = 1$：在根放入  $num$ 个球
2. $\rm op = 2$：拿走在位置 $num$ 的球

## 输出格式

1. $\rm op = 1$：输出最后一个球落到了哪里。
2. $\rm op = 2$：输出拿走那个球后有多少个球会掉下来。



```input1
8 4
0
1
2
2
3
3
4
6
1 8
2 5
2 7
2 8
```



```output1
1
3
2
2
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n, q \le  10^4$。

## 题目来源

abcdabcd987 提供

