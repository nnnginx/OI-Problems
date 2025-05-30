分值：$600$ 分

## 问题描述

Nagase 是一名高中优等生。有一天，她在分析一些特殊的正整数集合的性质。

她认为一个集合 $S = \{a_{1}, a_{2}, ..., a_{N}\}$ 被称为 **特殊** 的，如果对于所有 $1 \leq i \leq N$，$a_{i}$ 和集合 $S$ 中其余元素之和的最大公约数（gcd） **不** 为 1。

Nagase 想要找一个大小为 $N$ 的 **特殊** 集合。然而，这个任务对她来说太简单了，因此她决定提高难度。Nagase 向你挑战，要求你找一个大小为 $N$ 的 **特殊** 集合，使得所有元素的最大公约数为 1，并且集合中的元素不超过 30000。

## 约束条件

- $3 \leq N \leq 20000$

## 输入

输入通过标准输入提供，格式如下：

> $N$

## 输出

输出 $N$ 个用空格分隔的整数，表示集合 $S$ 的元素。$S$ 必须满足以下条件：

- 元素必须是 **不同** 的正整数，并且不超过 30000。
- $S$ 中所有元素的最大公约数为 1，即不存在一个大于 1 的整数 $d$ 能够整除 $S$ 中的所有元素。
- $S$ 是一个 **特殊** 集合。

如果有多个解法，你可以输出其中任何一个。集合 $S$ 的元素可以按任意顺序输出。保证在给定约束条件下至少存在一个解法。

```input1
3
```

```output1
2 5 63
```

$\{2, 5, 63\}$ 是特殊的，因为 $gcd(2, 5 + 63) = 2$，$gcd(5, 2 + 63) = 5$，$gcd(63, 2 + 5) = 7$。同时，$gcd(2, 5, 63) = 1$。因此，这个集合满足所有条件。

注意，$\{2, 4, 6\}$ 不是一个有效的解，因为 $gcd(2, 4, 6) = 2 > 1$。

```input2
4
```

```output2
2 5 20 63
```

$\{2, 5, 20, 63\}$ 是特殊的，因为 $gcd(2, 5 + 20 + 63) = 2$，$gcd(5, 2 + 20 + 63) = 5$，$gcd(20, 2 + 5 + 63) = 10$，$gcd(63, 2 + 5 + 20) = 9$。同时，$gcd(2, 5, 20, 63) = 1$。因此，这个集合满足所有条件。