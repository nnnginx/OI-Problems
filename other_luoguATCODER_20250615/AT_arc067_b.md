# AT_arc067_b [ABC052D] Walk and Teleport

## 题目描述

在东西方向延伸的直线上，有N个城市。城市坐标按从西到东递增。

你现在在某个城市里，想去其他所有的城市。移动的方法有以下两种。

一，在直线上按东西方向平移，每移动一个单位距离疲劳值加A

二，直接瞬移到某个坐标，并且疲劳值加B

请使用以上两种方式直到去完其他所有的城市，并求出最小的疲劳值。

## 输入格式

第一行三个数,即N,A,B,

第二行N个数，即X[1],X[2]...,X[N]。

## 输出格式

输出最小的疲劳值。

## 输入输出样例 #1

### 输入 #1

```
4 2 5
1 2 5 7
```

### 输出 #1

```
11
```

## 输入输出样例 #2

### 输入 #2

```
7 1 100
40 43 45 105 108 115 124
```

### 输出 #2

```
84
```

## 输入输出样例 #3

### 输入 #3

```
7 1 2
24 35 40 68 72 99 103
```

### 输出 #3

```
12
```

## 说明/提示

2<=N<=1e5

1<=Xi,A,B<=1e9且X(i)<X(i+1)