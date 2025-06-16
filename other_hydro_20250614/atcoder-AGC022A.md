分数：$300$ 分

## 问题描述

Gotou 刚刚收到了一本词典。然而，他无法识别词典中的语言。他对词典做了一些分析，并意识到词典中包含了所有可能的 **多样** 单词，并且这些单词是按字典序排列的。

一个单词被称为 **多样** 的，若且唯若它是一个非空的英文字母小写字母字符串，并且单词中的所有字母都是不同的。例如，`atcoder`、`zscoder` 和 `agc` 是多样单词，而 `gotou` 和 `connect` 不是多样单词。

给定一个多样单词 $S$，确定字典中在 $S$ 之后出现的下一个单词，即字典序中比 $S$ 大的最小的多样单词，或者确定这样一个单词不存在。

设 $X = x_{1}x_{2}...x_{n}$ 和 $Y = y_{1}y_{2}...y_{m}$ 为两个不同的字符串。如果 $X$ 在字典序中大于 $Y$，当且仅当 $Y$ 是 $X$ 的前缀，或者 $x_{j} > y_{j}$，其中 $j$ 是使得 $x_{j} \neq y_{j}$ 的最小整数。

## 约束条件

- $1 \leq |S| \leq 26$
- $S$ 是一个多样单词。

## 输入

输入通过标准输入提供，格式如下：

> $S$

## 输出

打印字典中在 $S$ 之后出现的下一个单词，如果不存在，则输出 `-1`。

```input1
atcoder
```

```output1
atcoderb
```

`atcoderb` 是字典序中比 `atcoder` 大的最小的多样单词。注意 `atcoderb` 的字典序比 `b` 小。

```input2
abc
```

```output2
abcd
```

```input3
zyxwvutsrqponmlkjihgfedcba
```

```output3
-1
```

这是字典序中最大的多样单词，因此答案是 `-1`。

```input4
abcdefghijklmnopqrstuvwzyx
```

```output4
abcdefghijklmnopqrstuvx
```