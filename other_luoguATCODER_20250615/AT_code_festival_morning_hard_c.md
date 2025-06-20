# AT_code_festival_morning_hard_c 宝探し 2

## 题目描述

**宝藏寻找 2**


太郎来到一个广场寻找宝藏。

这个广场被水平方向的 \( n \) 条线和垂直方向的 \( m \) 条线等间距地划分。相邻两条线之间的距离是 \( 1 \)。从上方数第 \( i \) 条水平线与从左侧数第 \( j \) 条垂直线相交的点的位置可以用坐标 (\( i \), \( j \)) 表示，在该点下埋藏着一种共 \( k \) 种之一的宝藏。

太郎拥有一台先进的机器，可以知道所有宝藏的埋藏位置和种类。因此，他打算调查广场上各种矩形区域内哪种宝藏的数量最多。

然而，次郎会时不时地恶作剧，将相邻的两个宝藏的位置交换。这里所说的相邻是指两处宝藏的埋藏点之间的距离恰好为 \( 1 \)。

请代替苦恼的太郎，对于给定的每个区域，找出其中数量最多的宝藏种类。

## 输入格式

输入以以下格式给出：

> \( n \) \( m \) \( k \) \( a_{1,1} \) \( a_{1,2} \) \( \ldots \) \( a_{1,m} \) \( \ldots \) \( a_{n,1} \) \( a_{n,2} \) \( \ldots \) \( a_{n,m} \) \( q \) \( t_1 \) \( x_{11} \) \( y_{11} \) \( x_{21} \) \( y_{21} \) \( \ldots \) \( t_q \) \( x_{1q} \) \( y_{1q} \) \( x_{2q} \) \( y_{2q} \)

* 第一行包含三个整数：表示广场上水平线条数的 \( n \)（\( 1 \leq n \leq 500 \)）、垂直线条数的 \( m \)（\( 1 \leq m \leq 500 \)）以及广场上宝藏种类数的 \( k \)（\( 1 \leq k \leq 100 \)）。
* 接下来的 \( n \) 行给出了广场上每个位置所埋藏的宝藏种类。
* \( a_{i,j} \)（\( 1 \leq a_{i,j} \leq k \)）表示广场上位置 (\( i \), \( j \)) 下所埋藏的宝藏种类。
* 在第 \( n + 2 \) 行有一个整数 \( q \)（\( 1 \leq q \leq 100,000 \)），表示查询的数量。
* 接下来的 \( q \) 行给出了每个查询的信息。
* \( t_i \)（\( 1 \leq t_i \leq 2 \)）表示第 \( i \) 个查询的类型。
* 当 \( t_i = 1 \) 时，表示第 \( i \) 个查询是由次郎发起的交换宝藏的查询，位置 (\( x_{1i} \), \( y_{1i} \)) 和位置 (\( x_{2i} \), \( y_{2i} \)) 上的宝藏会被交换。
* 当 \( t_i = 1 \) 时，位置 (\( x_{1i} \), \( y_{1i} \)) 和 (\( x_{2i} \), \( y_{2i} \)) 必定相邻。
* 当 \( t_i = 2 \) 时，表示第 \( i \) 个查询是调查当前宝藏状态的查询，需要统计位置 (\( x_{1i} \), \( y_{1i} \)) 和 (\( x_{2i} \), \( y_{2i} \)) 作为对角顶点的、与广场上的线条平行的矩形中的宝藏情况。
* 当 \( t_i = 2 \) 时，必定有 \( x_{1i} \leq x_{2i} \) 并且 \( y_{1i} \leq y_{2i} \)。
* 对于每个查询，都有 \( 1 \leq x_{1i}, x_{2i} \leq n \) 且 \( 1 \leq y_{1i}, y_{2i} \leq m \)。

## 输出格式

对于每个 \( t_i = 2 \) 的查询，输出该查询所表示的矩形区域内数量最多的宝藏种类及其数量，每组答案占一行。

如果数量最多的宝藏种类不止一种，则输出种类编号最大的那种。

最后不要有多余的字符或空行。

## 输入输出样例 #1

### 输入 #1

```
3 3 3
1 1 1
2 2 2
3 3 3
5
2 1 1 2 3
1 2 2 3 2
2 1 1 2 3
1 1 3 2 3
2 2 2 3 3
```

### 输出 #1

```
2 3
1 3
3 2
```

## 输入输出样例 #2

### 输入 #2

```
2 4 5
1 2 3 3
2 5 1 1
4
2 1 1 1 1
1 1 3 1 2
1 2 3 1 3
2 2 1 2 4
```

### 输出 #2

```
1 1
2 2
```