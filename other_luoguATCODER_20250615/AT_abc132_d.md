# AT_abc132_d [ABC132D] Blue and Red Balls

## 题目描述

有 $K$ 个蓝球和 $N-K$ 个红球。同一颜色的球是完全相同的。Snuke 和 Takahashi 在玩这些球。

首先，Snuke 将把 $N$ 个球从左到右排成一排。

然后，Takahashi 将收走 $K$ 个蓝球。在一次操作中，他可以收走连续的一个区间的蓝球。他将以最少的操作数收走所有蓝球。

Snuke 有多少种排列这 $N$ 个球的方法，使得 Takahashi 恰好操作 $i$ 次才能收走所有的 $K$ 个蓝球？对于每个 $i$（$1\le i\le K$）计算排列数对 $10^9+7$ 取模的结果。

------------

## 输入格式

$N\ K$

------------

## 输出格式

输出 $K$ 行。第 $i$ 行（$1\le i\le K$）表示有多少种排列这 $N$ 个球的方法，使得 Takahashi 恰好操作 $i$ 次才能收走所有的 $K$ 个蓝球，对 $10^9+7$ 取模。

------------

## 输入输出样例 #1

### 输入 #1

```
5 3
```

### 输出 #1

```
3
6
1
```

## 输入输出样例 #2

### 输入 #2

```
2000 3
```

### 输出 #2

```
1998
3990006
327341989
```

## 说明/提示

#### 样例解释 1
有三种方法来排列球，使得 Takahashi 恰好操作 $1$ 次：$(B, B, B, R, R)$，$(R, B, B, B, R)$ 和 $(R, R, B, B, B)$。（$R$ 和 $B$ 分别代表红色和蓝色）。

有六种方法来排列球，使得 Takahashi 恰好操作 $2$ 次：$(B, B, R, B, R)$，$(B, B, R, R, B)$，$(R, B, B, R, B)$，$(R, B, B, R, B)$，$(B, R, B, B, R)$，和 $(B, R, R, B, B)$。

有一种方法来排列球，使得 Takahashi 恰好操作 $3$ 次：$(B, R, B, R, B)$。

#### 样例解释 2
务必输出对 $10^9+7$ 的排列数。