## 题目描述

给出 $n$ 个长度为 $4$ 的字符串，问有且仅有 $d$ 处不相同的字符串有几对。

## 输入格式

第一行：$n,d$。

以下 $n$ 行每行一个字符串。

## 输出格式

一个数：有多少对有且仅有处不相同的字符串。

```input1
4 1
0000
a010
0202
a0e2
```
```output1
0
```

## 样例说明 1

For these PINs each pair of PINs differs at more than one position.

```input2
4 2
0000
a010
0202
a0e2
```
```output2
3
```

## 样例说明 2

There are three pairs that differ at exactly $2$ positions:

$(0000,a010),\\(0000,0202),\\(a010,a0e2)$

## 数据规模与约定

对于 $15\%$ 的数据，$n \leq 2\times10^3$。

对于 $30\%$ 的数据，$d=1$。

对于 $60\%$ 的数据，$d \leq 2$。

对于 $75\%$ 的数据，字符串中只包含小写字母 $a\sim f$ 以及 $0 \sim 9$。

对于 $100\%$ 的数据，$2 \leq n \leq 5 \times 10^4$，$1 \leq d \leq 4$，所有输入的字符串没有重复，串中的字符仅可能为 $a \sim z$ 或者 $0 \sim 9$。

## 题目来源

鸣谢 sachs