# AT_arc129_b [ARC129B] Range Point Distance

## 题目描述

对于一组整数 $l,r,x$，其中 $l \le r$，定义 $dist(l,r,x)$ 为：

- 若 $x < l$，则 $dist(l,r,x) = l - x$
- 若 $l \le x \le r$，则 $dist(l,r,x) = 0$
- 若 $x >r$，则 $dist(l,r,x) = x - r$ 

可以简要理解为 $x$ 在数轴上到区间 $[l,r]$ 的距离。

现在给定 $N$ 对整数，第 $i$ 对整数形如 $(L_i, R_i)$。对于 $k=1,2,\dots,N$，分别求解下面的问题：

- 自由选择一个整数 $x$，计算 $max_{i=1}^k dist(L_i,R_i,x)$，求其可能的最小值。

## 输入格式

第一行一个整数 $N$，表示给定 $N$ 对整数。

接下来 $N$ 行每行两个整数 $L_i,R_i$。

## 输出格式

共 $N$ 行，**依次输出** $k=1,2,\dots,N$ 时的答案，输出一个答案换一行。

## 输入输出样例 #1

### 输入 #1

```
3
1 3
2 4
5 6
```

### 输出 #1

```
0
0
1
```

## 输入输出样例 #2

### 输入 #2

```
10
64 96
30 78
52 61
18 28
9 34
42 86
11 49
1 79
13 59
70 95
```

### 输出 #2

```
0
0
2
18
18
18
18
18
18
21
```

## 说明/提示

- $1 \le N \le 2 \times 10^5$
- $1 \le L_i \le R_i \le 10^9$
- 所有输入均为整数。