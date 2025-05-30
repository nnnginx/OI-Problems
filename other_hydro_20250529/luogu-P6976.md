## 题目描述


You have a convex polygon. The vertices of the polygon are successively numbered from $1$ to $n$ . You also have a triangulation of this polygon, given as a list of $n − 3$ diagonals.

You are also given $q$ queries. Each query consists of two vertex indices. For each query, find the shortest distance between these two vertices, provided that you can move by the sides and by the given diagonals of the polygon, and the distance is measured as the total number of sides and diagonals you have traversed.



## 输入格式


The first line of the input file contains an integer $n$ -- the number of vertices of the polygon $(4 \le n \le 50 000)$ .

Each of the following $n−3$ lines contains two integers $a_{i}, b_{i}$ -- the ends of the i-th diagonal $(1 \le a_{i}, b_{i} \le n , a_{i} ≠ b_{i}).$

The next line contains an integer $q$ -- the number of queries $(1 \le q \le 100 000)$ .

Each of the following $q$ lines contains two integers $x_{i}, y_{i}$ -- the vertices in the i-th query $(1 \le x_{i}, y_{i} \le n)$ .

It is guaranteed that no diagonal coincides with a side of the polygon, and that no two diagonals coincide or intersect.



## 输出格式


For each query output a line containing the shortest distance.



## 题目大意
给定一个正 $n$ 边形及其三角剖分, 共 $2n−3$ 条边 ($n$ 条多边形的边和 $n−3$ 条对角线), 每条边的长度为 $1$。

共 $q$ 次询问, 每次询问给定两个点, 求它们的最短距离。

Translated by Eason_AC  
2020.11.19

```input1
6
1 5
2 4
5 2
5
1 3
2 5
3 4
6 3
6 6

```

```output1
2
1
1
3
0

```

## 提示
Time limit: 2 s, Memory limit: 256 MB. 



