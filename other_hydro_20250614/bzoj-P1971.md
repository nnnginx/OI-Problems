## 题目描述

Byteotian 基础服务政府准备研发一个计算机程序来帮助他们快速的找出两个城镇之间不同的路径。如果居民总是想找出最短的路径的话还是不难的。但是不幸的是，他们有时候想知道第 $k$ 短的路径。而且除此之外，路径中自环、重复经过点是允许的。如果两个城镇之间有 $4$ 条路径，他们的长度分别是 $2,4,4,5$，那么最短路径的长度为 $2$，次长为 $4$，第三长为 $4$，第四长的长度为 $5$。

## 输入格式

In the first line of the standard input there are two positive integers $n$ and $m$, separated by a single space. They are the number of towns in Byteotia and the number of roads connecting the towns, respectively. The towns are numbered from $1$ to $n$. 

In each of $m$ successive lines there are three integers separated by single spaces: $a, b$ and $l$, $a \neq b$. Each triple describes one one-way road of length $l$ enabling to move from the town $a$ to $b$. For each two towns there exist at most one road that enables to move in the given direction.

In the following line there is one integer $q$, denoting the number of queries. In the successive $q$ lines there are queries written, one per line. Each query has a form of three integers separated by single spaces: $c, d$ and $k$. Such a query refers to the length of the $k$-th shortest route from the town $c$ to the town $d$. 

输入文件的第一行有两个数 $n,m$，他们分别代表城镇总数和连接他们的道路总数。城镇编号从 $1$ 到 $n$。

接下来 $m$ 行，每行 $3$ 个整数：$a,b$ 和 $l$，它们代表一条长度为 $l$ 有向边从 $a$ 到 $b$。不会有两条边有着相同的起点和终点。

接下来一行是一个整数 $q$，代表一共有 $q$ 个询问。接下来 $q$ 行每行三个数：$c,d$ 和 $k$，表示询问城镇 $c$ 到城镇 $d$ 的第 $k$ 短路。

## 输出格式

对于每个询问，输出一行表示询问路径的长度，如果答案不存在，输出 `-1`.

```input1
5 5
1 2 3
2 3 2
3 2 1
1 3 10
1 4 1
8
1 3 1
1 3 2
1 3 3
1 4 2
2 5 1
2 2 1
2 2 2
1 1 2
```

```output1
5
8
10
-1
-1
3
6
-1
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 100$，$0 \le m \le n^2-n$，$1 \le l \le 500$，$1 \le q \le 10^4$，$1 \le k \le 100$。