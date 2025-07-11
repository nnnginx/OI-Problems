# AT_abc399_d [ABC399D] Switch Seats

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc399/tasks/abc399_d

$N$ 组数字对（称为“情侣对”）排成一列。  
请统计满足以下所有条件的 **两对不同的情侣对** $(a, b)$ 的组数：

1. 在原序列中，$a$ 的两个出现位置不邻接。
2. 在原序列中，$b$ 的两个出现位置不邻接。
3. 通过执行以下操作（次数不限），可以使 $a$ 的两个出现位置邻接，同时 $b$ 的两个出现位置也邻接：
   - 选择两个位置 $(i, j)$ 满足 $A_i = a$ 且 $A_j = b$，并交换这两个位置的值。

给定一个长度为 $2N$ 的序列 $A = (A_1, A_2, \dots, A_{2N})$，其中每个 $1, 2, \dots, N$ 恰好出现两次。  
对于 $T$ 个测试用例，分别输出答案。

## 输入格式

输入通过标准输入给出，格式如下：

> $T$  
> $\mathrm{case}_1$  
> $\mathrm{case}_2$  
> $\vdots$  
> $\mathrm{case}_T$

每个测试用例的格式为：

> $N$ $A_1$ $A_2$ $\dots$ $A_{2N}$

## 输出格式

输出 $T$ 行，每行对应一个测试用例的答案。

## 输入输出样例 #1

### 输入 #1

```
3
3
1 2 3 3 1 2
4
1 1 2 2 3 3 4 4
5
1 2 3 4 5 1 2 3 4 5
```

### 输出 #1

```
1
0
4
```

## 说明/提示

### 约束条件

- $1 \leq T \leq 2 \times 10^5$
- $1 \leq N \leq 2 \times 10^5$
- $1 \leq A_i \leq N$
- 每个 $1, 2, \dots, N$ 在 $A$ 中恰好出现两次
- 所有测试用例的 $N$ 总和不超过 $2 \times 10^5$
- 输入值均为整数

### 样例解释 1

考虑第一个测试用例 $(a, b) = (1, 2)$：
- 原序列中 $1$ 的两个出现位置不邻接。
- 原序列中 $2$ 的两个出现位置不邻接。
- 选择 $(i, j) = (1, 6)$ 交换 $A_1$ 和 $A_6$ 后，$1$ 的两个位置邻接，$2$ 的两个位置也邻接。  
因此满足条件的二元组 $(a, b)$ 仅有 $(1, 2)$ 这一组。

翻译由 DeepSeek R1 完成