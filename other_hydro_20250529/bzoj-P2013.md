## 题目描述

有 $n$ 块砖，要搭一个 $n$ 层的塔，要求：如果砖 $a$ 在砖 $b$ 上面，那么 $a$ 不能比 $b$ 的长度 $+ d$ 要长。问有几种方法，输出答案 $\bmod\ 10^9+9$ 的值。

## 输入格式

第一行：$n,d$。

第二行：$n$ 个数，表示每块砖的长度。

## 输出格式

方案数。输出要 $\bmod\ 10^9+9$。

```input1
4 1
1 2 3 100
```
```output1
4
```

## 样例说明 1

We can arrange the first three blocks in any order, except for $2,1,3$ or $1,3,2$. The last block has to be at the bottom.

```input2
6 9
10 20 20 10 10 20
```
```output2
36
```

## 样例说明 2

We are not allowed to put a cube of size $20$ onto a cube of size $10$.

There are six ways to order the cubes of size $10$, and six ways to order the cubes of size $20$.

## 数据规模与约定

对于 $10\%$ 的数据，$n \leq 10$。

对于 $30\%$ 的数据，方案数不超过 $10^6$。

对于 $45\%$ 的数据，$n \leq 20$。

对于 $70\%$ 的数据，$n \leq 70$。

对于 $100\%$ 的数据，$ 2 \leq n \leq 6.2\times 10^5$，输入中所有数字为不超过 $10^9$ 的正整数。