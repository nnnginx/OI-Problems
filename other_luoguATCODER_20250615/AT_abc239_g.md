# AT_abc239_g [ABC239G] Builder Takahashi

## 题目描述

给定一张 $n$ 个点 $m$ 条边的连通无向图，要求在某些点（不能为 $1$ 号点或者 $n$ 号点）设立障碍，在 $i$ 号点建立障碍的费用为 $c_i$，要使得 $1$ 号点和 $n$ 号点不连通，求最小花费的方案。

## 输入格式

第一行两个整数 $n,m(3\leq n\leq 100,n−1\leq m\leq \frac{n(n−1)}{2}−1)$。

接下来 $m$ 行，每行两个数 $a_i,b_i(1\leq ai < bi\leq n)$，保证没有重边自环，并且 $1$ 与 $n$ 不直接相连。

接下来一行 $n$ 个整数 $c_1,c_2,…,c_n(0\le ci\le 10^9)$，保证 $c_1=c_n=0$。

## 输出格式

第一行输出一个数，表示最小的花费。

接下来输出一个数 $k$，表示建立障碍的个数。接下来一行 $k$ 个数，表示建立障碍的 $k$ 个点。

## 输入输出样例 #1

### 输入 #1

```
5 5
1 2
2 3
3 5
2 4
4 5
0 8 3 4 0
```

### 输出 #1

```
7
2
3 4
```

## 输入输出样例 #2

### 输入 #2

```
3 2
1 2
2 3
0 1 0
```

### 输出 #2

```
1
1
2
```

## 输入输出样例 #3

### 输入 #3

```
5 9
1 2
1 3
1 4
2 3
2 4
2 5
3 4
3 5
4 5
0 1000000000 1000000000 1000000000 0
```

### 输出 #3

```
3000000000
3
2 3 4
```