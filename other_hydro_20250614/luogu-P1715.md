## 题目描述
Farmer John is thinking of selling some of his land to earn a bit of extra income. His property contains $N$ trees ($3 \leq N \leq 300$), each described by a point in the 2D plane, no three of which are collinear. FJ is thinking about selling triangular lots of land defined by having trees at their vertices; there are of course $L = \binom{N}{3}$ such lots he can consider, based on all possible triples of trees on his property.

A triangular lot has value $v$ if it contains exactly $v$ trees in its interior (the trees on the corners do not count, and note that there are no trees on the boundaries since no three trees are collinear). For every $v = 0 \ldots N-3$, please help FJ determine how many of his $L$ potential lots have value $v$.

## 输入格式
The first line of input contains $N$.

The following $N$ lines contain the $x$ and $y$ coordinates of a single tree; these are both integers in the range $0 \ldots 1,000,000$.

## 输出格式
Output $N-2$ lines, where output line $i$ contains a count of the number of lots having value $i-1$.

## 题目大意
### 题目描述

Farmer John 正在考虑出售他的一部分土地以赚取一些额外收入。他的财产包含 $N$ 棵树（$3 \leq N \leq 300$），每棵树由二维平面中的一个点描述，且任意三棵树不共线。FJ 正在考虑出售由三棵树作为顶点定义的三角形地块；显然，他可以考虑的此类地块数量为 $L = \binom{N}{3}$，基于他财产中所有可能的三棵树组合。

一个三角形地块的价值为 $v$，如果它的内部恰好包含 $v$ 棵树（顶点上的树不计入，且由于没有三棵树共线，边界上也没有树）。对于每个 $v = 0 \ldots N-3$，请帮助 FJ 确定他的 $L$ 个潜在地块中有多少个地块的价值为 $v$。

### 输入格式

输入的第一行包含 $N$。

接下来的 $N$ 行每行包含一棵树的 $x$ 和 $y$ 坐标；这些坐标都是 $0 \ldots 1,000,000$ 范围内的整数。

### 输出格式

输出 $N-2$ 行，其中第 $i$ 行输出价值为 $i-1$ 的地块数量。

```input1
7
3 6
17 15
13 15
6 12
9 1
2 7
10 19
```

```output1
28
6
1
0
0
```

