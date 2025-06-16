# AT_abc378_e [ABC378E] Mod Sigma Problem

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc378/tasks/abc378_e

You are given a sequence $A = (A_1, A_2, \dots, A_N)$ of $N$ non-negative integers, and a positive integer $M$.

Find the following value:

$$
 \sum_{1 \leq l \leq r \leq N} \left( \left(\sum_{l \leq i \leq r} A_i\right) \mathbin{\mathrm{mod}} M \right). 
$$

Here, $X \mathbin{\mathrm{mod}} M$ denotes the remainder when the non-negative integer $X$ is divided by $M$.

## 输入格式

The input is given from Standard Input in the following format:

> $N$ $M$
>
> $A_1$ $A_2$ $\dots$ $A_N$

## 输出格式

Print the answer.

## 输入输出样例 #1

### 输入 #1

```
3 4
2 5 0
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
10 100
320 578 244 604 145 839 156 857 556 400
```

### 输出 #2

```
2736
```

## 说明/提示

### 制約

### Constraints

-   $1 \leq N \leq 2 \times 10^5$
-   $1 \leq M \leq 2 \times 10^5$
-   $0 \leq A_i \leq 10^9$
 
### Sample Explanation 1

-   $A_1 \mathbin{\mathrm{mod}} M = 2$
-   $(A_1+A_2) \mathbin{\mathrm{mod}} M = 3$
-   $(A_1+A_2+A_3) \mathbin{\mathrm{mod}} M = 3$
-   $A_2 \mathbin{\mathrm{mod}} M = 1$
-   $(A_2+A_3) \mathbin{\mathrm{mod}} M = 1$
-   $A_3 \mathbin{\mathrm{mod}} M = 0$

The answer is the sum of these values, $10$. Note that the outer sum is not taken modulo $M$.