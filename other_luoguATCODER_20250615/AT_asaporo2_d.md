# AT_asaporo2_d Ancient Tree Record

## 题目描述

### 题目简述
Sunuke-kun 在古废墟中发现了一个共有 $N$ 顶点树的记录，他总结了他所观察的记录。

- 这棵树的顶端被编号为 $ 1,2,...,N $，侧面被编号为 $ 1,2,...,N-1 $。
- 边 $ i $ 由顶点 $ a_i $ 和 $ b_i $ 双向连接。
- 每边的长度是 $ 1 $ 和 $ 10^{18} $ 之间的整数
- 从顶点 $ i $ 到顶点 $ 1,...,N $ 的最短距离之和为 $ s_i $。

保证使用此信息可计算出每边的长度。此外，可以证明在这种情况下，每边的长度是唯一的。

## 输入格式

> $ N $ $ a_1 $ $ b_1 $ $ : $ $ a_{N-1} $ $ b_{N-1} $ $ s_1 $ $ s_2 $ $ ... $ $ s_{N} $

## 输出格式

输出共 $ N-1 $ 行，在第 $ i $ 行上输出边 $ i $ 的长度。

## 输入输出样例 #1

### 输入 #1

```
4
1 2
2 3
3 4
8 6 6 8
```

### 输出 #1

```
1
2
1
```

## 输入输出样例 #2

### 输入 #2

```
5
1 2
1 3
1 4
1 5
10 13 16 19 22
```

### 输出 #2

```
1
2
3
4
```

## 输入输出样例 #3

### 输入 #3

```
15
9 10
9 15
15 4
4 13
13 2
13 11
2 14
13 6
11 1
1 12
12 3
12 7
2 5
14 8
1154 890 2240 883 2047 2076 1590 1104 1726 1791 1091 1226 841 1000 901
```

### 输出 #3

```
5
75
2
6
7
50
10
95
9
8
78
28
89
8
```