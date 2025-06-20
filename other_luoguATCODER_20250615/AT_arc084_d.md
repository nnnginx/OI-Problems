# AT_arc084_d [ARC084F] XorShift

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc084/tasks/arc084_d

黑板上写有 $N$ 个非负整数。第 $i$ 个非负整数为 $A_i$。

高桥君可以按照任意顺序执行以下两种操作任意次数：

1. 选择黑板上写的一个整数，将该整数的 $2$ 倍的新整数添加到黑板上。被选中的整数仍保留在黑板上。
2. 选择黑板上写的不一定相异的两个整数，将这两个整数的按位异或（bitwise xor）得到的新整数添加到黑板上。被选中的整数仍保留在黑板上。

在黑板上可能出现的整数中，有多少种不超过 $X$ 的整数？注意，最初写在黑板上的整数也视为可能出现的整数。由于答案可能非常大，请输出其对 $998244353$ 取模的结果。

## 输入格式

输入通过标准输入给出，格式如下：

> $N$ $X$  
> $A_1$  
> $\vdots$  
> $A_N$

## 输出格式

输出黑板上可能出现的整数中不超过 $X$ 的整数的个数，对 $998244353$ 取模的结果。

## 输入输出样例 #1

### 输入 #1

```
3 111
1111
10111
10010
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
4 100100
1011
1110
110101
1010110
```

### 输出 #2

```
37
```

## 输入输出样例 #3

### 输入 #3

```
4 111001100101001
10111110
1001000110
100000101
11110000011
```

### 输出 #3

```
1843
```

## 输入输出样例 #4

### 输入 #4

```
1 111111111111111111111111111111111111111111111111111111111111111
1
```

### 输出 #4

```
466025955
```

## 说明/提示

### 约束条件

- $1 \leq N \leq 6$
- $1 \leq X < 2^{4000}$
- $1 \leq A_i < 2^{4000}$（$1 \leq i \leq N$）
- 输入均为整数
- $X$ 和 $A_i$（$1 \leq i \leq N$）以二进制形式给出，且最高位为 $1$

### 样例解释 #1

初始时，黑板上有 $15$、$23$ 和 $18$。在不超过 $7$ 的整数中，可以写出 $0$、$3$、$5$ 和 $6$ 这 $4$ 个数。例如，可以通过以下操作写出 $6$：
- 将 $15$ 乘以 $2$，得到 $30$ 并写在黑板上
- 对 $30$ 和 $18$ 取异或，得到 $12$ 并写在黑板上
- 将 $12$ 乘以 $2$，得到 $24$ 并写在黑板上
- 对 $30$ 和 $24$ 取异或，得到 $6$ 并写在黑板上

### 样例解释 #4

请输出对 $998244353$ 取模的结果。

翻译由 DeepSeek V3 完成