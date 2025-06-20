# AT_pakencamp_2018_day3_g 落単の危機

## 题目描述

## 题目翻译

高桥君需要在N天内提交一定的作业。

第$i$项作业的开始时间为第$E_i$天，截止时间为第$S_i$天，高桥君可以在这段时间内提交这份作业，每天，高桥君可以选择提交一份作业或不提交作业（不可提交两份或以上的作业）。高桥君每天都有一个“不想做”的值$X_i$。如果在第$i$天提交作业，总“不想做”值就会增加$X_i$。你要做的就是让总“不想做”值最小。

给定天数$N$，作业数量$M$和**至少**应该完成的作业数量$K$，你能帮助高桥君求出最小的总“不想做”值吗？

## 输入格式

第一行三个整数，分别是$N$，$M$和$K$。

第二行N个整数$X_i$，分别表示高桥君第$i$天的“不想做”值。

第$3$到$M+2$行，每行两个整数$S_i$和$E_i$，分别表示第$i$项作业的开始时间和截止时间。

## 输出格式

一个整数，表示总“不想做”值的最小值。

如果不能完成至少$K$项作业，输出$-1$。

## 输入输出样例 #1

### 输入 #1

```
4 3 2
5 6 3 7
1 1
2 3
3 4
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
5 5 5
8 6 9 1 20
1 2
3 4
5 5
4 5
3 5
```

### 输出 #2

```
-1
```

## 说明/提示

- $ 1\ \leq\ N\ \leq\ 1000 $
- $ 1\ \leq\ K\ \leq\ M\ \leq\ 1000 $
- $ 1\ \leq\ S_i\ \leq\ E_i\ \leq\ N $
- $ 1\ \leq\ X_i\ \leq\ 10^{9} $