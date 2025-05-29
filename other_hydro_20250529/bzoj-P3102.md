## 题目描述

Consider $n$ distinct points on a plane.Two points from that set are said to be friends, when there exists a rectangle with sides parallel to coordinate axes thatcontains those two points and doesn't contain any other point from the given set. A rectangle is said to contain a point if the point lies within the rectangle or on its border.

How many pairs of friends are there among the given points?

求这样的点对个数：以两点连线为对角线的矩形内不存在其他点（也不能在边界上）。

## 输入格式

The first line of the input file contains an integer $n$ .  
The next n lines contain two integers each, the coordinates of the given points. The coordinates don't exceed $10^9$ by absolute value.

## 输出格式

Output one integer number — the sought number of pairs of friends.


```input1
5
0 0
0 2
2 0
2 2
1 1
```


```output1
8
```
## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 10^5$ 。
