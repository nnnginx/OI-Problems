# AT_abc075_c [ABC075C] Bridge

## 题目描述

给你一个$N$个点$M$条边无重边无自环的无向图。

求有几个桥（自行百度）。

## 输入格式

第一行两个正整数$N,M$，之后$M$行每行两个数$u,v$描述无向边。

## 输出格式

一个正整数代表图里有几个桥。

## 输入输出样例 #1

### 输入 #1

```
7 7
1 3
2 7
3 4
4 5
4 6
5 6
6 7
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
3 3
1 2
1 3
2 3
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
6 5
1 2
2 3
3 4
4 5
5 6
```

### 输出 #3

```
5
```

## 说明/提示

$1 \leq N \leq 50$

$N-1 \leq M \leq N(N-1)/2$