## 题目描述
Let $T$ be a rooted tree (a connected undirected acylic graph), and let $S$ be a perfect copy of $T$. Construct a new graph by taking the union of $T$ and $S$, and merging the corresponding leaf nodes (but never the root). We call such a graph a tree-mirrored graph.

## 输入格式
The first line of input contains two integers $N$ and $M$, the number of vertices and edges of a graph $G$. The vertices in $G$ are labeled from $1$ to $N$. The following $M$ lines describe the edges. Each such line contains two integers $x$ and $y(x≠y;1 \le x,y \le N)$, describing one edge. There will be at most one edge between any pair of vertices.

## 输出格式
The first and only line of output should contain the string ``YES`` if the graph $G$ is a tree-mirrored graph, and ``NO`` otherwise.

## 题目大意
### 题目描述

对于一棵树 $T$，并复制一棵与 $T$ 同构的树 $S$。构造一个新的图 $T'$，新图 $T'$ 通过合并 $T$ 和 $S$ 中相应的非根叶节点得到。我们称这样的图为树之镜像图。

给定一个图 $G$，你需要判断 $G$ 是否是树之镜像图。

### 输入输出格式

#### 输入格式：

输入的第一行包含两个整数 $N$ 和 $M$，表示图 $G$ 的顶点和边数。

接下来有 $M$ 行，每一行包含两个正整数 $x$ 和 $y$（$x \neq y$ 且 $1 \leq x,y \leq n$）表示顶点 $x$ 和 $y$ 之间有一条边。保证没有重边。

#### 输出格式：

输出只有一行，判断图 $G$ 是否是一个树之镜像图，是输出 `yes`，否则输出 `no`。

Translated by @找寻 

```input1
7 7
1 2
2 3
3 4
4 5
5 6
6 7
7 1
```

```output1
NO
```

```input2
6 6
1 2
2 3
2 4
3 5
4 5
5 6
```

```output2
YES
```

```input3
22 28
13 8
8 1
1 22
1 12
1 14
13 18
13 4
4 20
20 7
13 15
15 3
15 9
9 16
9 19
22 5
12 5
14 5
5 11
11 6
18 6
7 10
10 17
17 6
3 21
21 6
16 2
19 2
2 21
```

```output3
YES
```

## 提示
对于 $30\%$ 的数据，$3 \le N,M \le 300$。

对于 $60\%$ 的数据，$3 \le N,M \le 3500$。

对于所有数据，$3 \le N,M \le 10^5$。

