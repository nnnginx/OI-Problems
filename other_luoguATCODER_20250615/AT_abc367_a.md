# AT_abc367_a [ABC367A] Shout Everyday

## 题目描述

### 问题描述

在 AtCoder 王国里，居民们会在每天的 $A$ 点钟大声表达对章鱼小丸子的爱。

居住在 AtCoder 王国的高桥君每天会在 $B$ 点睡觉并在 $C$ 点醒来。当高桥君醒着的时候他可以表达对章鱼小丸子的爱，而当他睡着的时候则不能。请判断高桥君是否每天都能表达对章鱼小丸子的爱。注意一天有 $24$ 小时，并且高桥君睡觉的时间少于 $24$ 小时。

## 输入格式

输入以以下格式从标准输入给出:

> $A$ $B$ $C$

## 输出格式

如果高桥君每天都能表达对章鱼小丸子的爱，则输出 `Yes`；否则输出 `No`。

### 约束条件

- $0 \leq A, B, C < 24$
- $A$, $B$, 和 $C$ 各不相同
- 所有输入均为整数

#### 示例解释 1

高桥君每天在 $8$ 点睡觉并在 $14$ 点醒来。因为他在 $21$ 点是醒着的，所以他每天都能表达对章鱼小丸子的爱。因此输出 `Yes`。

#### 示例解释 2

高桥君每天在 $21$ 点睡觉并在 $7$ 点醒来。由于他在 $0$ 点是睡着的，所以他无法每天表达对章鱼小丸子的爱。因此输出 `No`。

## 输入输出样例 #1

### 输入 #1

```
21 8 14
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
0 21 7
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
10 7 17
```

### 输出 #3

```
No
```