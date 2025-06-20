# AT_tkppc4_1_o Height Changer

## 题目描述

今年的 Paken 训练营有 $N$ 名成员参加。所有成员已经到达了讲堂，讲堂左边有一块正在使用的幻灯片屏幕。由于讲堂空间有限，成员们只能从左到右排成一排。此时，他们从左到右依次被编号为 $1$ 到 $N$。

在这个团体中，成员们的排列根据离幻灯片的远近及评分高低的顺序确定，所以无法改变队列顺序。然而，不同成员的身高各有差异，这导致个头较矮的成员可能看不到屏幕。

为了解决这个问题，魔法少年 Osmium\_1008 决定使用一种魔法来缩小部分成员的身高（他可以将身高缩小，但无法增加）。

第 $i$ 位成员的身高为 $A_i$，成功看到幻灯片时的快乐值为 $B_i$。如果在他左侧的成员中，有任何一位的身高比他高（**相等的情况不算**），那么这个成员将无法看到幻灯片，快乐值将变为 $0$。另外，如果 Osmium\_1008 动用魔法，把某位成员的身高缩小了，则该成员的快乐值还会因为身高缩小量而减少。

请你计算出所有成员的快乐值总和的最大值。值得注意的是，Osmium\_1008 可以选择不使用魔法，而且每个成员的快乐值可能是负值。

## 输入格式

输入信息从标准输入中按以下格式给出：

> $ N $  
> $ A_1 $ $ A_2 $ $ \ldots $ $ A_{N-1} $ $ A_N $  
> $ B_1 $ $ B_2 $ $ \ldots $ $ B_{N-1} $ $ B_N $

## 输出格式

请输出所有成员快乐值总和的最大值，以一行表示。

## 输入输出样例 #1

### 输入 #1

```
4
40 60 20 10
25 30 80 50
```

### 输出 #1

```
95
```

## 输入输出样例 #2

### 输入 #2

```
5
112 76 50 35 22
15 60 40 120 90
```

### 输出 #2

```
140
```

## 输入输出样例 #3

### 输入 #3

```
5
151 162 155 161 170
4 8 23 10 15
```

### 输出 #3

```
53
```

## 说明/提示

- 所有输入均为整数。
- $1 \leq N \leq 10^5$
- $1 \leq A_i, B_i \leq 10^9$

### 子任务

1. (400 分) $N \leq 5000$
2. (600 分) 没有其他额外约束条件。

 **本翻译由 AI 自动生成**