## 题目描述

You are given $K$ points with positive integer coordinates. You are also given $M$ triangles, each of them having one vertex in the origin and the other $2$ vertices with non-negative integer coordinates.

You are asked to determine for each triangle whether it has at least one of the $K$ given points inside. (None of the $K$ points are on any edge of any triangle.)

## 输入格式

The first line will contain $K$ and $M$.

The following $K$ lines will contain $2$ positive integers $x,y$ separated by one space that represent the coordinates of each point.

The next $M$ lines have $4$ non-negative integers separated by one space, $(x_1,y_1)$ and $(x_2,y_2)$, that represent the other $2$ vertices of each triangle, except the origin.

## 输出格式

The output should contain exactly $M$ lines. The $k^{th}$ line should contain the character `Y` if the $k^{th}$ triangle (in the order of the input file) contains at least one point inside it, or `N` otherwise.

## 样例

```input1
4 3
1 2
1 3
5 1
5 3
1 4 3 3
2 2 4 1
4 4 6 3 
```

```output1
Y
N
Y
```

```input2
4 3
1 2
1 3
5 1
5 3
1 4 3 3
2 2 4 1
4 4 6 3 
```

```output2
Y
N
Y
```

## 样例说明

![](./1319/file/pic1.png) ![](./1319/file/pic2.png)

## 数据规模与约定

In $50\%$ of the test cases, all triangles have vertices with coordinates $x_1=0$ and $y_2=0$. That is, one edge of the triangle is on the x-axis, and another is on the y-axis.

In $100\%$ of the test cases, $1\leq K,M\leq 10^5$, $1\leq\text{each coordinate of the } K \text{ points}\leq 10^9$, $0\leq\text{each coordinate of the triangle vertices}\leq 10^9$, Triangles are not degenerate (they all have nonzero area).

## 题目来源

Ceoi2009