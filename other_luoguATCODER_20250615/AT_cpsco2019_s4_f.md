# AT_cpsco2019_s4_f Lost Tree

## 题目描述

拉斯克君曾经拥有一棵美丽的树，不过，他现在把它弄丢了。

这棵树的每个顶点都有一个从 $1$ 到顶点总数之间的独特编号，每条边也都有一个从 $1$ 到 $10^9$ 间的整数权重。

树的顶点数在 $K$ 和 $1000$ 之间。对于任意两个顶点 $i$ 和 $j$（$1 \leq i, j \leq K$），它们之间的距离用 $D_{ij}$ 表示。在这里，顶点间的距离是指连接这两个顶点的简单路径上所有边的权重之和。

根据这些给定的信息，请输出一种可能的树结构，该树是拉斯克君遗失的树。题目保证，对于提供的输入，总可以找到至少一种符合条件的树。

## 输入格式

输入以如下格式呈现：

> $K$ $D_{11}$ $D_{12}$ $\ldots$ $D_{1K}$ $D_{21}$ $D_{22}$ $\ldots$ $D_{2K}$ : $D_{K1}$ $D_{K2}$ $\ldots$ $D_{KK}$

## 输出格式

请以如下格式输出一种符合条件的树：

> $N$ $a_1$ $b_1$ $c_1$ $a_2$ $b_2$ $c_2$ : $a_{N-1}$ $b_{N-1}$ $c_{N-1}$

其中，$N$ 表示顶点数，$a_i$ 和 $b_i$ 是通过一条权重为 $c_i$ 的边直接相连的顶点，这个数据描述了一棵符合要求的树。

如果有多棵符合条件的树，输出其中任意一棵即可。

注意，边的权重 $c_i$ 必须是 $1$ 到 $10^9$ 之间的整数。

## 输入输出样例 #1

### 输入 #1

```
4
0 3 4 5
3 0 5 6
4 5 0 7
5 6 7 0
```

### 输出 #1

```
5
1 5 1
4 5 4
5 2 2
5 3 3
```

## 输入输出样例 #2

### 输入 #2

```
3
0 2 3
2 0 5
3 5 0
```

### 输出 #2

```
4
1 4 1
1 2 2
4 3 2
```

## 输入输出样例 #3

### 输入 #3

```
5
0 5 6 3 5
5 0 7 6 6
6 7 0 7 3
3 6 7 0 6
5 6 3 6 0
```

### 输出 #3

```
8
4 6 2
6 1 1
2 7 3
7 8 2
7 6 1
5 8 1
8 3 2
```

## 说明/提示

- 输入的所有数值均为整数。
- $2 \leq K \leq 300$
- 对于 $i \neq j$ 的情况，$1 \leq D_{ij} \leq 10^9$
- 距离满足对称性：$D_{ij} = D_{ji}$
- 每个顶点到自身的距离为零：$D_{ii} = 0$
- **题目确保至少存在一棵满足条件的树。**

### 样例解释 1

例如，下图所示的树符合条件：
![示例 1](https://img.atcoder.jp/cpsco2019-s4/cf49e2d95234dcb394eec3b9185455a6.png)

### 样例解释 2

例如，下图所示的树符合条件：
![示例 2](https://img.atcoder.jp/cpsco2019-s4/937c00db989f458f17a3ad78d4b30c76.png)

 **本翻译由 AI 自动生成**