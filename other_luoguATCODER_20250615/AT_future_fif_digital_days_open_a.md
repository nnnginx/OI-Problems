# AT_future_fif_digital_days_open_a future_fif_digital_days_open_a

## 题目描述

在一个 $N \times N$ 的棋盘上，有 $B$ 种多连块。这些多连块可以放置在棋盘上，使得被它们覆盖的区域变为可通行。棋盘上有 $K$ 个格子被标记，初始时所有格子都是不可通行的。我们的目标是通过放置多连块，使得所有标记格子连通。

例如，在下面的图中，中间两个标记是连通的，但上面的标记与下面的不连通。

![](https://img.atcoder.jp/future-fif-digital-days/b490bb01158a72323fc4b1072acff8ef.svg)

多连块不能旋转，不能超出棋盘边界，也不能重叠放置。每种多连块 $b$ 都有一个放置费用 $C_b$。当使用 $m_b$ 个多连块 $b$ 时，总费用为 $\sum_{b=1}^B C_b m_b$。请尽可能减少费用，使所有标记格子连成一片。

## 输入格式

从标准输入中按如下格式获取输入：

> $N$ $K$ $B$  
> $i_1$ $j_1$  
> $\vdots$  
> $i_K$ $j_K$  
> $n_1$ $m_1$ $C_1$  
> $s^1_{1,1}$ $\ldots$ $s^1_{1,m_1}$  
> $\vdots$  
> $s^1_{n_1,1}$ $\ldots$ $s^1_{n_1,m_1}$  
> $\vdots$  
> $n_B$ $m_B$ $C_B$  
> $s^B_{1,1}$ $\ldots$ $s^B_{1,m_B}$  
> $\vdots$  
> $s^B_{n_B,1}$ $\ldots$ $s^B_{n_B,m_B}$

- 第1行包含整数 $N$、$K$ 和 $B$，分别表示棋盘大小、标记格子数目和多连块种类数。所有测试用例中，$N$ 固定为 50。
- 接下来的 $K$ 行，每行包含一对整数 $(i_p, j_p)$，表示第 $p$ 个标记格子的坐标，满足 $0 \leq i_p \leq N-1$ 和 $0 \leq j_p \leq N-1$，并且这些坐标是互不相同的。
- 接下来的部分描述每种多连块的详细信息：
  - $n_b$ 和 $m_b$ 是第 $b$ 种多连块的最小包围矩形（bounding box）的高度和宽度。保证 $n_1 = m_1 = 1$。
  - $C_b$ 表示放置一个第 $b$ 种多连块的费用，是一个正整数。
  - $s^b_{i,j}$ 表示第 $b$ 种多连块在其边界内第 $i$ 行、第 $j$ 列的信息。`#` 表示是多连块的一部分，`.` 表示不是。

每个多连块都是连通的。

## 输出格式

输出格式如下：第一行输出你使用的多连块总数 $m$，接下来 $m$ 行，每行给出一个多连块的种类编号 $b_i$ 和其左上角坐标 $(x_i, y_i)$。

> $m$  
> $b_1$ $x_1$ $y_1$  
> $\vdots$  
> $b_m$ $x_m$ $y_m$

## 输入输出样例 #1

### 输入 #1

```
50 70 11
0 0
35 0
49 14
8 49
0 2
1 19
41 31
30 18
3 8
44 10
32 42
27 27
0 27
17 3
28 18
17 48
4 13
1 21
17 17
10 25
14 16
35 36
19 7
25 12
6 46
25 24
18 32
31 47
15 12
41 15
24 16
49 22
49 17
29 42
30 32
22 8
36 39
9 12
7 7
20 46
16 15
17 34
16 21
17 28
46 4
26 21
45 17
10 32
26 35
45 31
40 45
28 45
0 20
17 22
45 9
33 34
39 20
46 20
30 5
10 48
9 37
26 37
29 30
29 46
41 19
0 4
4 47
6 37
36 2
2 25
1 1 1
#
7 4 2
####
#...
#...
###.
#...
#...
#...
4 5 2
#...#
#...#
#...#
#####
8 3 2
###
.#.
.#.
.#.
.#.
.#.
.#.
.#.
4 5 2
####.
#..##
####.
#..##
5 4 2
####
#...
###.
#...
####
4 4 2
####
#..#
#..#
####
5 8 3
#......#
#......#
########
#......#
#......#
8 7 3
..###..
.##.##.
##...##
#.....#
#######
#.....#
#.....#
#.....#
8 8 3
..######
.##.....
##......
#.......
#.......
##......
.##.....
..######
9 6 3
#....#
#...##
#..##.
#.##..
###...
#.##..
#..##.
#...##
#....#
```

### 输出 #1

```
326
1 0 0
1 0 1
1 0 2
1 0 3
1 0 4
1 1 19
1 1 20
1 1 21
1 0 20
1 30 18
1 29 18
1 28 18
1 44 10
1 44 9
1 45 9
1 16 21
1 16 22
1 17 22
1 26 35
1 26 36
1 26 37
1 28 45
1 28 46
1 29 46
1 35 0
1 35 1
1 35 2
1 36 2
1 49 14
1 49 15
1 49 16
1 49 17
1 8 49
1 8 48
1 9 48
1 10 48
1 32 42
1 31 42
1 30 42
1 29 42
1 17 17
1 16 17
1 16 16
1 16 15
1 14 16
1 15 16
1 6 46
1 5 46
1 4 46
1 4 47
1 18 32
1 17 32
1 17 33
1 17 34
1 31 47
1 30 47
1 29 47
1 30 32
1 29 32
1 29 31
1 29 30
1 39 20
1 39 19
1 40 19
1 41 19
1 9 37
1 8 37
1 7 37
1 6 37
1 41 31
1 42 31
1 43 31
1 44 31
1 45 31
1 0 27
1 0 26
1 0 25
1 1 25
1 2 25
1 35 36
1 35 37
1 35 38
1 35 39
1 36 39
1 34 36
1 33 36
1 33 35
1 33 34
1 19 7
1 19 8
1 20 8
1 21 8
1 22 8
1 25 24
1 25 23
1 25 22
1 25 21
1 26 21
1 15 12
1 15 13
1 15 14
1 15 15
1 41 15
1 41 16
1 41 17
1 41 18
1 48 17
1 47 17
1 46 17
1 45 17
1 28 42
1 28 43
1 28 44
1 46 18
1 46 19
1 46 20
1 7 48
1 6 48
1 6 47
1 3 8
1 3 7
1 4 7
1 5 7
1 6 7
1 7 7
1 27 27
1 26 27
1 25 27
1 25 26
1 25 25
1 27 28
1 27 29
1 27 30
1 28 30
1 27 18
1 26 18
1 26 19
1 26 20
1 17 48
1 17 47
1 17 46
1 18 46
1 19 46
1 20 46
1 1 22
1 1 23
1 1 24
1 16 18
1 16 19
1 16 20
1 25 12
1 24 12
1 24 13
1 24 14
1 24 15
1 24 16
1 17 31
1 17 30
1 17 29
1 17 28
1 49 22
1 48 22
1 47 22
1 46 22
1 46 21
1 30 33
1 30 34
1 31 34
1 32 34
1 3 9
1 3 10
1 3 11
1 3 12
1 3 13
1 4 13
1 17 3
1 17 4
1 17 5
1 17 6
1 17 7
1 18 7
1 25 18
1 24 18
1 24 17
1 4 12
1 5 12
1 6 12
1 7 12
1 8 12
1 9 12
1 14 12
1 13 12
1 12 12
1 11 12
1 10 12
1 42 17
1 43 17
1 44 17
1 17 27
1 17 26
1 17 25
1 17 24
1 17 23
1 46 4
1 45 4
1 45 5
1 45 6
1 45 7
1 45 8
1 10 32
1 9 32
1 9 33
1 9 34
1 9 35
1 9 36
1 2 7
1 1 7
1 0 7
1 0 6
1 0 5
1 32 41
1 32 40
1 32 39
1 33 39
1 34 39
1 16 48
1 15 48
1 14 48
1 13 48
1 12 48
1 11 48
1 10 25
1 10 26
1 10 27
1 10 28
1 10 29
1 10 30
1 10 31
1 23 12
1 22 12
1 22 11
1 22 10
1 22 9
1 29 34
1 28 34
1 27 34
1 26 34
1 44 11
1 44 12
1 44 13
1 44 14
1 44 15
1 44 16
1 15 11
1 15 10
1 15 9
1 15 8
1 15 7
1 16 7
1 9 25
1 8 25
1 7 25
1 6 25
1 5 25
1 4 25
1 3 25
1 16 25
1 15 25
1 14 25
1 13 25
1 12 25
1 11 25
1 21 46
1 22 46
1 23 46
1 24 46
1 25 46
1 26 46
1 27 46
1 30 5
1 30 4
1 30 3
1 30 2
1 31 2
1 32 2
1 33 2
1 34 2
1 36 40
1 36 41
1 36 42
1 36 43
1 36 44
1 36 45
1 37 45
1 38 45
1 39 45
1 40 45
1 40 31
1 39 31
1 38 31
1 37 31
1 36 31
1 35 31
1 34 31
1 33 31
1 33 32
1 33 33
1 30 19
1 31 19
1 32 19
1 33 19
1 34 19
1 35 19
1 36 19
1 37 19
1 38 19
1 22 7
1 22 6
1 22 5
1 23 5
1 24 5
1 25 5
1 26 5
1 27 5
1 28 5
1 29 5
```

## 说明/提示

### 得分

总费用为 $S$ 时，得分为 $\mathrm{round}(10^8 / S)$。如果输出不正确（标记格子不连通，多连块超出棋盘边界或重叠），将被判定为错误。若有任何测试未通过，总得分为0。最终排名由比赛中的最高分决定，比赛结束后不进行验证测试。平分时先提交者排名更高。

### 测试用例数量

1个

### 输入生成方式

A问题的测试用例数量为1，与输入示例1相同。可以提前计算结果并提交。

### 工具

- [在线可视化及输入生成器](https://img.atcoder.jp/future-fif-digital-days/visYp.html?q=a)
- [本地运行版可视化及输入生成器](https://img.atcoder.jp/future-fif-digital-days/dd7a70773bb74f0570cdde81b1bf6ee3.zip)：需先安装 [Rust](https://www.rust-lang.org/ja) 编译环境。

 **本翻译由 AI 自动生成**