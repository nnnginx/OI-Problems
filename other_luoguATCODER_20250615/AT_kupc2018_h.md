# AT_kupc2018_h カラフル数列

## 题目描述

托尔君是个非常喜欢数列的男孩。

在一次日常地欣赏数列时，他听到了电视里提到“多样性”这个词语。

受此启发，托尔君想为自己的数列增添多样性。因此，他决定创建一个由 $N$ 个整数组成的数列 $a_1, a_2, \ldots, a_N$，需要满足以下条件：

- 对于每个 $i$ ($1 \leq i \leq M$)，子序列 $a_{l_i}, a_{l_i + 1}, \ldots, a_{r_i}$ 中至少要有一个数字与 $b_i$ 不同。
- 所有数列元素的值必须在 $1$ 和 $S$ 之间（包括 $1$ 和 $S$）。

托尔君对满足这些条件的数列数量产生了好奇，但发现自己无法手动计算出结果。

请帮助托尔君计算能够满足这些条件的数列的总数。由于结果可能十分巨大，请输出对 $10^9 + 7$ 取模后的答案。

## 输入格式

输入以如下格式给出：

> $N$ $M$ $S$ $l_1$ $r_1$ $b_1$ $l_2$ $r_2$ $b_2$ $\ldots$ $l_M$ $r_M$ $b_M$

## 输出格式

输出满足上述条件的数列的总数，并对 $10^9 + 7$ 取模。

## 数据范围

- 所有输入均为整数。
- $1 \leq N \leq 2 \times 10^5$
- $1 \leq M \leq 2 \times 10^5$
- $1 \leq S \leq 10^5$
- $1 \leq l_i \leq r_i \leq N$
- $1 \leq b_i \leq S$
- 每个 $(l_i, r_i, b_i)$ 组合都是唯一的。

### 样例解释

需要满足的条件如下：
- 在 $a_1, a_2$ 中，至少有一个数字不是 $1$。
- 在 $a_2, a_3$ 中，至少有一个数字不是 $2$。
- 数列中的每个数字必须介于 $1$ 和 $2$ 之间。

可以满足这些条件的数列有：$(1, 2, 1)$, $(2, 1, 1)$, $(2, 1, 2)$, $(2, 2, 1)$，共计 $4$ 种。

 **本翻译由 AI 自动生成**

## 输入输出样例 #1

### 输入 #1

```
3 2 2
1 2 1
2 3 2
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
8 3 4
1 5 1
2 6 1
4 8 1
```

### 输出 #2

```
65364
```

## 输入输出样例 #3

### 输入 #3

```
7 6 4
1 5 1
3 6 3
2 2 4
5 7 4
4 7 2
2 2 3
```

### 输出 #3

```
7984
```

## 输入输出样例 #4

### 输入 #4

```
5 3 52657
1 2 1
4 5 1
1 5 1
```

### 输出 #4

```
145394311
```

## 输入输出样例 #5

### 输入 #5

```
8 10 3
1 5 1
6 8 2
2 6 2
3 7 1
8 8 3
1 3 3
4 8 1
5 6 3
3 7 2
1 8 2
```

### 输出 #5

```
3439
```