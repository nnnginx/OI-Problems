# AT_past202005_e スプリンクラー

## 题目描述

有一个 $n$ 点 $m$ 边的无向图。点的编号依次为 $1$ 到 $n$ ，边的编号依次为 $1$ 到 $m$ 。现在以 $i=1,2,...,m$ 的顺序给出 $i$ 号边连接的两个点的编号 $u_i$ 和 $v_i$ 。数据保证给定的图中没有重边和自环。

开始时，每个顶点都涂有一种颜色，记编号 $i$ 的点涂有的颜色为 $c_i$ （本题中 $1≤c_i≤10^5$ 且 $c_i$ 为整数）。

## 输入格式

- `1 x`：输出点 $x$ 的颜色，并将所有与 $x$ 点有边相连的点的颜色全部替换为 $x$ 点的颜色。
- `2 x y`：输出点 $x$ 的颜色，并用颜色 $y$ 覆盖当前顶点 $x$ 的颜色。

请按照 $i=1,2,...,q$ 的顺序处理 $s_i$ 。


输入 $(m+q+2)$ 行。

第一行：三个非负整数 $n,m,q$ 。

第二行至第 $(m+1)$ 行：第 $(i+1)$ 行包含两个正整数 $u_i,v_i$ ，表示边 $i$ 连接点 $u_i$ 和 $v_i$ 。

第 $(m+2)$ 行： $n$ 个正整数 $c_1,c_2,...,c_n$ ，即各个点的原始颜色。

## 输出格式

输出 $q$ 行。每行一个正整数，第 $i$ 行输出 $s_i$ 中询问的点（即 $x_i$ ）在操作前的颜色。

## 输入输出样例 #1

### 输入 #1

```
3 2 3
1 2
2 3
5 10 15
1 2
2 1 20
1 1
```

### 输出 #1

```
10
10
20
```

## 输入输出样例 #2

### 输入 #2

```
30 10 20
11 13
30 14
6 4
7 23
30 8
17 4
6 23
24 18
26 25
9 3
18 4 36 46 28 16 34 19 37 23 25 7 24 16 17 41 24 38 6 29 10 33 38 25 47 8 13 8 42 40
2 1 9
1 8
1 9
2 20 24
2 26 18
1 20
1 26
2 24 31
1 4
2 21 27
1 25
1 29
2 10 14
2 2 19
2 15 36
2 28 6
2 13 5
1 12
1 11
2 14 43
```

### 输出 #2

```
18
19
37
29
8
24
18
25
46
10
18
42
23
4
17
8
24
7
25
16
```