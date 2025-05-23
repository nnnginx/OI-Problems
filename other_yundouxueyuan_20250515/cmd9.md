# 修路

## 题目描述

奶龙有一个 $n$ 个点 $m$ 条边的无向图，每条边连接顶点 $u_i,v_i$ ，距离为 $w_i$。

奶龙现在计划在原无向图基础上, 再修 $k$ 条双向道路，这些路径起点都是 $1$ 号点，终点是 $1$ 号点外的其他顶点。假设修了这些路后，从 $1$ 号点到其他点的最短距离为 $dis_i$ ，奶龙想知道，最多可以少修几条路，少修哪些路，使得从 $1$ 号点到其他点的最短距离仍然为 $dis_i$ 。

## 输入格式

第一行三个整数 $n,m,k$ 表示点数，边数，奶龙原本计划修的路数。

接下来 $m$ 行，每行三个整数 $u_i,v_i,w_i$ ，表示一条边的两个端点以及权值。

接下来 $k$ 行，每行两个整数 $t_i,d_i$ ，表示计划修从 $1$ 号点到 $t_i$ 号点的一条路，长度为 $d_i$ 。

## 输出格式

第一行一个整数 $c$ 表示最多可以少修的路的数量。

第二行 $c$ 个整数表示这些少修的路的编号，编号从小到大输出，如果存在多种方案，请输出任意方案。

## 样例 #1

### 样例输入 #1

```
3 2 2
1 2 3
2 3 1
2 2
3 3
```

### 样例输出 #1

```
1
2
```

## 样例 #2

### 样例输入 #2

```
9 10 4
1 2 8
1 3 12
2 4 13
1 5 7
2 6 5
6 7 11
4 8 4
8 9 10
1 4 5
2 3 20
4 2
5 8
6 13
9 1
```

### 样例输出 #2

```
2
2 3
```

## 提示

对于样例1，$d_1=0,d_2=2,d_3=3$ ，删除第 $2$ 条边之后距离不变。

对于 $20\%$ 的数据，满足 $n \le 10,m \le 20$ 。

对于另外 $10\%$ 的数据，满足 $n \le 100,m \le 200$ 。

对于另外 $20\%$ 的数据，满足 $n \le 1000,m \le 2000$ 。

对于另外 $20\%$ 的数据，满足 $n \le 100000,m \le 200000,k=1$ 。

对于全部数据，满足 $1\le n \le 100000,1 \le m \le 200000,0 \le k \lt n,1 \le w_i,d_i \le 10^9,1 \le u_i,v_i \le n,u_i \neq v_i,t_i \neq 1$ 。

输入保证图联通，即从 $1$ 号点出发能到达任何点，而且 $t_i$ 互不相同。
