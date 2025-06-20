# AT_arc090_b [ABC087D] People on a Line

## 题目描述

在一根数轴上站有 $n$ 个人，我们称第 $i$ 个人的坐标为 $x_i(x_i\in [0,10^{9}],x_i\in Z)$，同一个坐标点上可能有多个人。

你现在手上有 $m$ 条信息，第 $i$ 条信息形如 $(li,ri,di)$，含义是第 $r_i$ 个人在第 $l_i$ 个人右数第 $d_i$ 个坐标点上，换言之，$x_{r_i} - x_{l_i} = d_i$。

不幸的是，这 $m$ 条信息中的一些可能有误，请你求出是否存在一组 $x (x_1,x_2,x_3,\dots ,x_n)$ 满足所有信息。

## 输入格式

输入数据的第一行包含两个以空格分开的整数 $n$ 和 $m$，分别表示总人数和信息条数；

接下来的 $m$ 行中第 $i(1\le i\le m)$ 行包含三个以空格分开的整数 $l_i,r_i,d_i$，表示第 $i$ 条信息是 $r_i$ 号人在 $l_i$ 号人右边 $d_i$ 个位置上。

## 输出格式

若存在一组合法的 $x$，输出一行 ``Yes``；否则输出一行 ``No``。

## 输入输出样例 #1

### 输入 #1

```
3 3
1 2 1
2 3 1
1 3 2
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
3 3
1 2 1
2 3 1
1 3 5
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
4 3
2 1 1
2 3 5
3 4 2
```

### 输出 #3

```
Yes
```

## 输入输出样例 #4

### 输入 #4

```
10 3
8 7 100
7 9 100
9 8 100
```

### 输出 #4

```
No
```

## 输入输出样例 #5

### 输入 #5

```
100 0
```

### 输出 #5

```
Yes
```

## 说明/提示

全部的输入数据满足以下条件：

-  $1 \le n \le 100000$；
-  $0 \le m \le 200000$；
- $1\le l_i,r_i\le n (1\le i\le m)$；
- $0\le d_i\le 10000 (1\le i\le m)$；
- $l_i \ne r_i (1 \le i \le m)$；
- 如果 $i\le j$，则有 $(l_i,r_i)\ne (l_j,r_j),(l_i,r_i)\ne (r_j,l_j)$；
- $d_i$ 为整数。


$(0,1,2)$ 与 $(101,102,103)$ 都是合法的解。


若前两条信息是正确的，则有 $x_3 - x_1 = 2$，那么第三条信息就是错误的。

感谢@fbhou  提供的翻译