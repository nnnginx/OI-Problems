# AT_pakencamp_2021_day3_b レートで2分割！

## 题目描述

有 $N$ 名帕研部的成员被安排在一个圆环上，按照顺时针方向依次编号为 $1$ 到 $N$。

每个成员有一个“评分”，记为 $A_i$，代表编号为 $i$ 的成员的评分。

帕研部长——企鹅君，有一个想法：他想将这 $N$ 名成员划分为两个连续的组，并且希望其中一个组的成员评分总和为 $X$，另一个组的成员评分总和为 $Y$。

你的任务是判断是否可以实现这种划分。

## 输入格式

输入从标准输入读取，包含：

> $ N $ $ X $ $ Y $ $ A_1 $ $ A_2 $ $\ldots$ $ A_N $

## 输出格式

如果可以按题目要求将 $N$ 名成员划分为两组，则输出 `Yes`；否则输出 `No`。

## 输入输出样例 #1

### 输入 #1

```
5 6 11
3 4 2 3 5
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
4 4 8
1 2 3 4
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
10 191 376
72 6 62 98 90 61 36 82 9 51
```

### 输出 #3

```
Yes
```

## 说明/提示

- **约束条件：**
  - $2 \leq N \leq 2 \times 10^5$
  - $1 \leq X, Y \leq 10^{15}$
  - $1 \leq A_i \leq 10^9$（此处所有 $A_i$ 均为整数）

- **子任务：**
  1. ($100$ 分) $N \leq 3000$
  2. ($200$ 分) 没有额外的限制条件

### 示例解析 1：

将第 $2$ 位和第 $3$ 位成员分为一组，其他成员分为另一组，那么这两组成员的评分总和分别是 $X=6$ 和 $Y=11$。该输入满足所有子任务条件。

### 示例解析 2：

无法根据题目要求将 $N$ 名成员划分为两个组。该输入仍然符合所有子任务的条件。。

### 示例解析 3：

该输入满足所有子任务条件。题目来源：[penguinman](https://atcoder.jp/users/penguinman)

 **本翻译由 AI 自动生成**