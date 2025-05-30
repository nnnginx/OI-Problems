## 题目描述

给定一个包含 $n$ 个结点和 $m$ 条带权边的无向连通图 $G=(V,E)$。 

再给定包含 $k$ 个结点的点集 $S$，选出 $G$ 的子图 $G'=(V',E')$，使得： 

1. $S \subseteq V'$； 
2. $G'$ 为连通图； 
3. $E'$ 中所有边的权值和最小。 你只需要求出 $E'$ 中所有边的权值和。

## 输入格式

第一行包含三个整数 $n,m,k$，表示 $G$ 的结点数、边数和 $S$ 的大小。 

接下来 $m$ 行，每行三个整数 $u,v,w$，表示编号为 $u,v$ 的点之间有一条权值为 $w$ 的无向边。 

接下来一行包含 $k$ 个互不相同的正整数，表示 $S$ 的元素。

## 输出格式

一行一个整数，表示 $E'$ 中边权和的最小值。

```input1
7 7 4
1 2 3
2 3 2
4 3 9
2 6 2
4 5 3
6 5 2
7 6 4
2 4 7 5
```

```output1
11
```

## 数据范围与提示

对于 $100 \%$ 的数据，$1 \leq n \leq 100$，$1 \leq m \leq 500$，$1 \leq k \leq 10$，$1 \leq u,v \leq n$，$1 \leq w \leq 10^6$。 

保证给出的无向图连通，应该不存在重边和自环。

