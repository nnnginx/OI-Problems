# AT_past202004_n ビルの建設

## 题目描述

平面直角坐标系上有 $n$ 个正方形，第 $i$ 个正方形的左下角坐标为 $(xmin_i,ymin_i)$，边长为 $d_i$。每个正方形都有一个值 $c_i$。

有 $q$ 次询问，第 $i$ 次询问给出一个坐标 $(a_i,b_i)$，请计算覆盖此点的所有正方形的 $c$ 之和。

## 输入格式

第一行为两个整数 $n,q$。

接下来 $n$ 行，每行四个整数 $xmin_i,ymin_i,d_i,c_i$。

接下来 $q$ 行，每行两个整数 $a_i,b_i$。

## 输出格式

输出 $q$ 行，第 $i$ 行输出第 $i$ 个询问的结果。

## 输入输出样例 #1

### 输入 #1

```
2 4
1 3 6 10
3 6 6 20
4 7
-1 -1
1 4
7 13
```

### 输出 #1

```
30
0
10
0
```

## 输入输出样例 #2

### 输入 #2

```
2 3
-3 5 4 100
1 9 7 30
1 9
1 8
8 10
```

### 输出 #2

```
130
100
30
```

## 输入输出样例 #3

### 输入 #3

```
10 10
17 2 17 1000000000
7 12 12 1000000000
2 12 8 1000000000
2 12 2 1000000000
3 9 16 1000000000
8 13 15 1000000000
8 1 3 1000000000
15 9 17 1000000000
16 5 5 1000000000
13 12 9 1000000000
17 3
4 10
1 9
5 3
17 12
14 19
19 17
17 11
16 17
12 16
```

### 输出 #3

```
1000000000
1000000000
0
0
5000000000
4000000000
6000000000
3000000000
5000000000
3000000000
```

## 说明/提示

#### 数据规模与约定

- $1 \le n \le 50000$，$1 \le q \le 100000$；
- $|xmin_i|,|ymin_i|,|a_i|,|b_i| \le 10^9$，$1 \le d_i \le 10^9$，$0 \le c_i \le 10^9$（样例 #3 证明了结果可能会爆`int`）。