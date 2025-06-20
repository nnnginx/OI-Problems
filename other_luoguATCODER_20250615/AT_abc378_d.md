# AT_abc378_d [ABC378D] Count Simple Paths

## 题目描述

给定一个 $H$ 行 $W$ 列的网格；令 $(i, j)$ 为网格中从上到下第 $i$ 行、从左到右第 $j$ 列的格子。 

当 $ S_{i,j} $ 为 `.` 时，格子为空格；当 $ S_{i,j} $ 为 `#` 时，格子为障碍物。

请计算从某个空格出发，经过 $K$ 次移动（上下左右），不经过障碍物且不重复经过同一个格子的路径数。

具体地，统计满足以下条件的，长度为 $K+1$ 的序列 $((i_0,j_0),(i_1,j_1),\dots,(i_K,j_K))$

- 对于每个 $ 0\ \leq\ k\ \leq\ K $，都有 $ 1\ \leq\ i_k\ \leq\ H,\ 1\ \leq\ j_k\ \leq\ W $，且 $ S_{i_k,j_k} $ 为 `.`。
- 对于每个 $ 0\ \leq\ k\ \leq\ K-1 $，有 $ |i_{k+1}-i_k|\ +\ |j_{k+1}-j_k|\ =\ 1 $。
- 对于每个 $ 0\ \leq\ k\ <\ l\ \leq\ K $，有 $ (i_k,j_k)\neq\ (i_l,j_l) $。

## 输入格式

输入为标准输入，格式如下：

>$ H $ $ W $ $ K $
$ S_{1,1}S_{1,2}\dots S_{1,W} $
$ S_{2,1}S_{2,2}\dots S_{2,W} $
$\vdots$
$ S_{H,1}S_{H,2}\dots S_{H,W} $

## 输出格式

输出满足条件的路径数量。

### 样例1 解释


总共有两种可能的路径

-   $(1,1) \rightarrow (2,1) \rightarrow (2,2)$
-   $(2,2) \rightarrow (2,1) \rightarrow (1,1)$


Translated by [Route101](https://www.luogu.com.cn/user/262435).

## 输入输出样例 #1

### 输入 #1

```
2 2 2
.#
..
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
2 3 1
.#.
#.#
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
10 10 11
....#..#..
.#.....##.
..#...##..
...#......
......##..
..#......#
#........#
..##......
.###....#.
...#.....#
```

### 输出 #3

```
218070
```

## 说明/提示

-  $1 \leq H, W \leq 10$
-  $1 \leq K \leq 11$
-  $H$, $W$, 和 $K$ 均为整数。
-  每个 $S_{i,j}$ 均为 `.` 或 `#`。
-  网格中至少存在一个格子为空格。