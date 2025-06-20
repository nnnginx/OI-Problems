# AT_arc192_d [ARC192D] Fraction Line

## 题目描述

对于正有理数 $x$，定义 $f(x)$ 如下：

> 当 $x$ 用互质的正整数 $P, Q$ 表示为 $\dfrac{P}{Q}$ 时，$f(x)$ 的值为 $P \times Q$

给定正整数 $N$ 和长度为 $N-1$ 的正整数序列 $A = (A_1, A_2, \dots, A_{N-1})$。

我们称满足以下所有条件的长为 $N$ 的正整数序列 $S = (S_1, S_2, \dots, S_N)$ 为**好序列**：

- 对于所有满足 $1 \leq i \leq N-1$ 的整数 $i$，有 $f\left(\dfrac{S_i}{S_{i+1}}\right) = A_i$
- $\gcd(S_1, S_2, \dots, S_N) = 1$

定义序列的**分数**为该序列所有元素的乘积。

可以证明好序列的个数是有限的。请计算所有好序列的分数之和对 $998244353$ 取模的结果。

## 输入格式

输入通过标准输入给出，格式如下：

> $N$ $A_1$ $A_2$ $\dots$ $A_{N-1}$

## 输出格式

输出所有好序列的分数之和对 $998244353$ 取模的结果。

## 输入输出样例 #1

### 输入 #1

```
6
1 9 2 2 9
```

### 输出 #1

```
939634344
```

## 输入输出样例 #2

### 输入 #2

```
2
9
```

### 输出 #2

```
18
```

## 输入输出样例 #3

### 输入 #3

```
25
222 299 229 22 999 922 99 992 22 292 222 229 992 922 22 992 222 222 99 29 92 999 2 29
```

### 输出 #3

```
192457116
```

## 说明/提示

### 约束条件

- $2 \leq N \leq 1000$
- $1 \leq A_i \leq 1000$ $ (1 \leq i \leq N-1)$
- 输入均为整数

### 样例解释 1

例如 $(2, 2, 18, 9, 18, 2)$ 和 $(18, 18, 2, 1, 2, 18)$ 是好序列，它们的分数均为 $23328$。共有 $16$ 个好序列，所有好序列的分数之和为 $939634344$。

### 样例解释 2

共有 $2$ 个好序列，它们的分数均为 $9$。

### 样例解释 3

请勿忘记将总和对 $998244353$ 取模。

翻译由 DeepSeek R1 完成