分数 : $700$ 分

## 问题陈述

有 $N$ 个字符串排列成一行。
已知，对于任何两个相邻的字符串，左边的字符串在字典序上小于右边的字符串。
也就是说，$S_1$ 在字典序上小于 $S_2$，以此类推，其中 $S_i$ 是从左边数的第 $i$ 个字符串。

如果已知 $S_i$ 的长度为 $A_i$，那么 $S_1,S_2,...,S_N$ 至少包含多少个不同的字符？

## 约束条件

- $1 \leq N \leq 2\times 10^5$
- $1 \leq A_i \leq 10^9$
- $A_i$ 是一个整数。

## 注意

这些字符串不一定由英文字母组成；可以有任意多的不同字符（并且这些字符的字典序是有定义的）。

## 输入

输入通过标准输入以以下格式给出：

> $N$
> 
> $A_1$ $A_2$ $...$ $A_N$

## 输出

打印字符串中包含的最小不同字符的数量。

```input1
3
3 2 1
```

```output1
2
```

例如，当 $S_1=$`abc`，$S_2=$`bb` 和 $S_3=$`c` 时，$S_1,S_2,...,S_N$ 中包含的不同字符数量为 $3$。

然而，如果我们适当选择字符串，不同字符的数量可以是 $2$。

```input2
5
2 3 2 1 2
```

```output2
2
```