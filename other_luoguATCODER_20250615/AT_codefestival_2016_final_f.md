# AT_codefestival_2016_final_f Road of the King

## 题目描述

有一个 $n$ 个点的图，目前一条边都没有。

有一个人在 $1$ 号点要进行 $m$ 次移动，终点不必是 $1$ 号点，假设第 $i$ 次从 $u$ 移动到 $v$，那么在 $u$ 与 $v$ 之间连一条有向边。

问有多少种序列能满足：最终 $n$ 个点组成的图是一个强连通图。答案对 $10^9+7$ 取模。

## 输入格式

> $n$$\ m$

两个整数 $n,m$，用一个空格隔开。

## 输出格式

> $ans$

一个整数表示答案。

## 输入输出样例 #1

### 输入 #1

```
3 3
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
150 300
```

### 输出 #2

```
734286322
```

## 输入输出样例 #3

### 输入 #3

```
300 150
```

### 输出 #3

```
0
```

## 说明/提示

$1 \leq n,m \leq 300$