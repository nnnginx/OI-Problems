# AT_tkppc4_2_e 引きこもり

## 题目描述

给定一张 $N$ 点 $M$ 边的无向图。顶点的编号从 $1$ 到 $N$，第 $i$ 条边连接点 $A_i$ 和点 $B_i$，长度为 $C_i$。

有 $Q$ 组询问，第 $i$ 组询问会给出一个整数 $q_i$。请找出满足条件的最小的非负整数 $L$，使得将图中长度不大于 $L$ 的边加粗后，称由加粗的边连接的几个点在同一连通块内，则每个连通块内点的个数均不小于 $q_i$。若不存在这样的整数 $L$，请输出 `trumpet`。

## 输入格式

第一行输入三个整数 $N,M,Q$。

第二行开始的 $M$ 行，每行输入三个整数 $A_i,B_i,C_i$，表示第 $i$ 条边连接的两个顶点的编号及其长度。

最后 $Q$ 行，第 $i$ 行输入单个整数 $q_i$，表示第 $i$ 次询问的参数。

## 输出格式

输出 $Q$ 行，第 $i$ 行输出第 $i$ 个询问的答案。

### 输入输出样例

#### 输入 #1

```
9 10 4
1 2 3
1 4 1
3 4 4
2 3 1
4 5 9
5 6 3
6 7 4
7 8 2
8 9 3
6 9 5
2
3
5
10

```

#### 输出 #1

```
3
4
9
trumpet

```

## 输入输出样例 #1

### 输入 #1

```
9 10 41 2 31 4 13 4 42 3 14 5 95 6 36 7 47 8 28 9 36 9 523510
```

### 输出 #1

```
349trumpet
```

## 说明/提示

#### 样例 #1 解释

![样例 #1 解释](https://img.atcoder.jp/tkppc4-2/faff237ade903a85fd7554c7f343687e.png)

以第一次询问为例，红色的边为加粗的边。可以看出 $3$ 满足条件，$2$ 不满足。

#### 数据规模与约定

对于全部测试点，保证：

- $2\le N,M,Q\le 10^5$；
- $1\le A_i,B_i\le N$，$0\le C_i\le 10^{10}$；
- $1\le q_i\le 10^5$。

**不保证** 给出的图是简单连通无向图。