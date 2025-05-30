## 题目描述
You are given $n$ vertical lines with x-coordinates $x_1, x_2, \ldots, x_n$ and weights $a_1, a_2, \ldots, a_n$ and $m$ horizontal lines with y-coordinates $y_1, y_2, \ldots, y_m$ and weights $b_1, b_2, \ldots, b_m$.

Call a rectangle good if and only if all of its four edges lie on the given lines. On this basis, define the cost of a good rectangle as the sum of the costs of its four segments. The cost of a segment is the product of its length and the weight of the line it belongs.

Find the maximum area of good rectangles with cost no more than $c$. Note that the length and the width of the rectangle can be zero, so the answer always exists.

You need to answer $T$ queries with different $c$.

## 输入格式
The first line contains three integers $n$, $m$ ($2\leq n, m\leq 5\,000$) and $T$ ($1\leq T\leq 100$).

The second line contains $n$ integers $x_1, x_2, \ldots, x_n$ ($1\leq x_1 < x_2 < \ldots < x_n \leq 10 ^ 5$).

The third line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1\leq a_i\leq 10 ^ 7$).

The fourth line contains $m$ integers $y_1, y_2, \ldots, y_m$ ($1\leq y_1 < y_2 < \ldots < y_m \leq 10 ^ 5$).

The fifth line contains $m$ integers $b_1, b_2, \ldots, b_m$ ($1\leq b_i\leq 10 ^ 7$).

Each of the next $T$ lines contains a single integer $c$ ($1\leq c\leq 4\times 10 ^ {12}$), representing a query.

## 输出格式
For each query, output one line representing the answer.

## 题目大意
### 题目描述：
给定 $n$ 条垂直的线和 $m$ 条水平线，每条线有重量。定义一个矩形是好的，当且仅当矩形的四个边都落在这些线上，好矩形的代价等于其内部四条边的长度与对应线重量的乘积之和。请找出最大面积的好矩形，使得其代价不超过 $c$。注意，矩形的长度和宽度可以为零。

### 输入格式：
第一行三个正整数 $n,m,T(2 \leq n, m \leq 5 \times 10^3, 1 \leq T \leq 100)$，依次表示垂直线、水平线的数量以及查询的次数。

第二行 $n$ 个正整数 $x_1,x_2,\cdots,x_n(1 \leq x_1 < x_2 < \cdots < x_n \leq 10^5)$，其中 $x_i$ 表示第 $i$ 条垂直线的位置。

第三行 $n$ 个正整数 $a_1,a_2,\cdots,a_n$，其中 $a_i$ 表示第 $i$ 条垂直线的重量。

第四行 $m$ 个正整数 $y_1,y_2,\cdots,y_m(1 \leq y_1 < y_2 < \cdots < y_m \leq 10^5)$，其中 $y_i$ 表示第 $i$ 条水平线的位置。

第五行 $m$ 个正整数 $b_1,b_2,\cdots,b_m(1 \leq b_i \leq 10^7)$，其中 $b_i$ 表示第 $i$ 条水平线的重量。

接下来 $T$ 行，每行一个正整数 $c(1 \leq c \leq 4\times 10^{12})$，表示一次查询。

### 输出格式：
对于每次查询，输出一个整数表示最小代价不超过 $c$ 的最大好矩形的面积。

translated by @[cff_0102](/user/542457)

```input1
3 4 20
1 3 4
3 1 2
1 3 4 7
4 2 1 2
1
5
6
7
9
10
11
12
15
16
17
22
23
28
30
35
43
47
49
57

```

```output1
0
0
1
1
1
2
2
3
3
4
4
6
6
9
9
12
12
12
18
18

```

## 提示
**Source**: The 2022 ICPC Asia Xi'an Regional Contest Problem K.

**Author**: Alex_Wei.

