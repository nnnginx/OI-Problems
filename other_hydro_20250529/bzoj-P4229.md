

## 题目描述

现在，我想知道自己是否还有选择。

给定 $n$ 个点 $m$ 条边的无向图以及顺序发生的 $q$ 个事件。

每个事件都属于下面两种之一：

1. 删除某一条图上仍存在的边
2. 询问是否存在两条边不相交的路径可以从点 $u$ 出发到点 $v$
## 输入格式

第一行三个整数$n,m,q$

接下来 $m$ 行，每行两个整数 $u,v$ ，表示 $u$ 和 $v$ 之间有一条边

接下来 $q$ 行，每行一个大写字母 $o$ 和2个整数 $u,v$ ，依次表示按顺序发生的q个事件：

当 $o$ 为 $Z$ 时，表示删除一条 $u$ 和 $v$ 之间的边

当 $o$ 为 $P$ 时，表示询问是否存在两条边不相交的路径可以从点 $u$ 出发到点 $v$

## 输出格式
对于每组询问，如果存在，输出Yes,否则输出No

```input1
7 8 7
1 2
1 3
1 4
2 3
3 4
3 7
7 4
5 6
Z 1 4
P 1 3
P 2 4
Z 1 3
P 1 3
Z 6 5
P 5 6

```

```output1
Yes
Yes
No
No
```

## 数据规模与约定

对于 $100\% $ 数据，$\max_{n,m,q} \le 10^5$


