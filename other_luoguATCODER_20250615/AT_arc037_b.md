# AT_arc037_b [ARC037B] バウムテスト

## 题目描述

给出由 $N$ 个顶点和 $M$ 条边构成的无向图表。求出该图表中的像树一样的部分，即不具有闭路的部分的个数。

## 输入格式

第 $1$ 行表示无向图表中包含的顶点数 $N$ 和边的数量 $M$。

接下来的第 $2$ 行到第 $M+1$ 行，第 $i$ 行输入连接两个顶点的编号 $u_i$ 与 $v_i$。

## 输出格式

一行，输出无向图表的树的个数。

## 输入输出样例 #1

### 输入 #1

```
8 7
1 2
2 3
2 4
5 6
6 7
6 8
7 8
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
5 1
1 2
```

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
11 11
1 2
1 3
2 4
3 5
4 6
5 7
6 8
7 9
8 10
9 11
10 11
```

### 输出 #3

```
0
```

## 说明/提示

($ 2 $ $ ≦ $ $ N $ $ ≦ $ $ 100 $) 

($ 1 $ $ ≦ $ $ M $ $ ≦ $ $ N×(N-1)/2 $)

($ 1 $ $ ≦ $ $ i $ $ ≦ $ $ M $)

($ 1 $ $ ≦ $ $ u_i $ $ ＜ $ $ v_i $ $ ≦ $ $ N $) 

值得注意的是：对于任何两个顶点，直接连接它们的边最多只有一条。