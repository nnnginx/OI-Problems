# AT_abc127_e [ABC127E] Cell Distance

## 题目描述

有一个 $n \times m$ 的矩形，你会从中选出 $k$ 个坐标为整数的位置 $(x_1,y_1),(x_2,y_2)\dots(x_{k},y_{k})$ 。

你定义一个选出 $k$ 个位置的方案的权值为$\textstyle \sum_{i=1}^{k-1}\sum_{j=i+1}^{k}(|x_{i}-x_{j}|+|y_{i}-y_{j}|)$

你需要求出，所有可能的选出 $k$ 个位置的方案的权值之和，答案对 $1000000007$ 取模

## 输入格式

一行三个整数 $n,m,k$

## 输出格式

一行一个整数，表示答案

## 输入输出样例 #1

### 输入 #1

```
2 2 2
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
4 5 4
```

### 输出 #2

```
87210
```

## 输入输出样例 #3

### 输入 #3

```
100 100 5000
```

### 输出 #3

```
817260251
```

## 说明/提示

$2 \le k \le n \times m \le 200000$