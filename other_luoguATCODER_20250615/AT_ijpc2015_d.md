# AT_ijpc2015_d 格子点

## 题目描述

对多边形内的格子点很感兴趣的 Snuke 君，自从学会了 Pick 定理后，对格子点就不那么迷恋了。

为了让 Snuke 君重新燃起兴趣，Sune 君设计了一个别具一格的平面。

这个平面是 $xy$ 平面中的一个区域，满足 $x, y \ge 0$。在这个区域中，每个格子点 $(a, b)$ 都被赋予了一个值，该值代表从 $(0, 0)$ 出发，只通过格子点向上或者向右移动，到达 $(a, b)$ 的路径数量，即组合数 $\binom{a+b}{a}$。

Snuke 君对这个平面喜欢得不行，于是不断地向 Sune 君提出各种问题。

Snuke 君问：「被平面的边界（两个坐标轴）和直线 $ax + by = c$ 围成的直角三角形内及其边界上的所有格子点，对应值的总和是多少？」

Sune 君回答：「别提那么大的数，你也算不出来。稍安勿躁。」

Snuke 君坚持：「好好好，那你告诉我结果对 $1000000007$ 取模后是多少！」

Sune 君没想到 Snuke 君会如此热衷。请你代为解答 Snuke 君的问题吧。

## 输入格式

输入通过标准输入提供，格式如下：

> $Q$
> $a_1$ $b_1$ $c_1$
> ...
> $a_Q$ $b_Q$ $c_Q$

- 第一行一个整数 $Q (1 \le Q \le 1000000)$，表示查询的数量。
- 接下来的 $Q$ 行，每行三个整数 $a_i, b_i, c_i (1 \le a_i, b_i, c_i \le 10000)$，表示每个查询中的直线 $a_i x + b_i y = c_i$。

## 输出格式

对于每个查询，输出一行，表示对应直角三角形内及其边界上的格子点值的总和，最后结果需对 $1000000007$ 取模。每个输出结果后需要换行。

 **本翻译由 AI 自动生成**

## 输入输出样例 #1

### 输入 #1

```
3
7 10 8
6 3 6
1 5 2
```

### 输出 #1

```
2
4
3
```

## 输入输出样例 #2

### 输入 #2

```
5
10 4 7
8 1 3
4 4 7
1 10 5
8 8 5
```

### 输出 #2

```
2
4
3
6
1
```