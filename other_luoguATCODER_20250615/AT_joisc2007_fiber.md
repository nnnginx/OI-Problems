# AT_joisc2007_fiber 光ファイバー (Fiber)

## 题目描述

### 题目简述

有一张 $n$ 点 $m$ 边的无向图，问最少再连多少条边使得图连通。若图连通，输出 $0$ 即可。

## 输入格式

第一行输入顶点个数 $n$。

第二行输入边的条数 $m$。

第三行到第 $(m+2)$ 行，第 $(i+2)$ 行输入两个整数 $a_i,b_i$，表示边 $i$ 连接的两个顶点的编号。

## 输出格式

一行一个整数，最少所需连的边的条数。

### 输入输出样例

#### 输入 #1

```
8
7
3 5
4 1
5 4
7 5
4 7
1 4
6 8
```

#### 输出 #1

```
2
```

## 说明/提示

#### 样例 #1 解释

例如，可以连接点 $2$ 和点 $1$，以及点 $6$ 和点 $4$。

#### 数据规模与约定

- 对于 $100\%$ 的测试点，保证 $1\le n\le 10000$，$1\le m\le 30000$，$1\le a_i,b_i\le n$，$a_i\neq b_i$。