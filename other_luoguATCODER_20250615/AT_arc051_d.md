# AT_arc051_d [ARC051D] 長方形

## 题目描述

给定一个长度为 $W$ 的数列 $a_1, a_2, \ldots, a_W$ 和一个长度为 $H$ 的数列 $b_1, b_2, \ldots, b_H$。

现在，我们构造一个 $W \times H$ 的矩阵。矩阵中第 $i$ 列第 $j$ 行的格子的值为 $a_i + b_j$。

接下来有 $Q$ 个查询，每个查询要求如下：

- 给定两个参数 $A$ 和 $B$，请在左上角 $A$ 列以内和 $B$ 行以内的所有格子中选择一些格子，要求这些格子组成一个矩形，并求出这些格子的值之和的最大值。注意，至少需要选择一个格子。

## 输入格式

输入从标准输入读取，格式如下：

> $W\ H\ a_1\ a_2\ \ldots\ a_W\ b_1\ b_2\ \ldots\ b_H\ Q\ A_1\ B_1\ A_2\ B_2\ \ldots\ A_Q\ B_Q$

其中，$A_i$ 和 $B_i$ 分别是第 $i$ 个查询的参数 $A$ 和 $B$。

## 输出格式

输出 $Q$ 行，每行一个整数，对应每个查询的最大值结果。结果按照查询给出的顺序输出。

## 数据范围
- $1 \leq W, H \leq 2000$
- $1 \leq Q \leq 2000$
- $1 \leq A \leq W$
- $1 \leq B \leq H$
- $-100,000 \leq a_i, b_i \leq 100,000$

 **本翻译由 AI 自动生成**

## 输入输出样例 #1

### 输入 #1

```
2 2
0 10
0 -1
4
1 1
1 2
2 1
2 2
```

### 输出 #1

```
0
0
10
19
```

## 输入输出样例 #2

### 输入 #2

```
3 3
1 10 100
1000 10000 100000
9
1 1
1 2
1 3
2 1
2 2
2 3
3 1
3 2
3 3
```

### 输出 #2

```
1001
11002
111003
2011
22022
222033
3111
33222
333333
```

## 输入输出样例 #3

### 输入 #3

```
10 8
2 -4 0 0 -1 4 5 0 -3 0
2 0 0 -3 -5 -5 -4 -4
10
2 6
1 4
1 2
5 7
1 5
7 6
7 4
1 5
3 5
10 7
```

### 输出 #3

```
8
8
6
8
8
34
34
8
8
36
```