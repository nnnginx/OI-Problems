得分 : $600$ 分

## 问题陈述

给定一个长度为 $2N$ 的字符串 $S$，由小写英文字母组成。

每个字符可以用红色或蓝色着色，共有 $2^{2N}$ 种方式。在这些方式中，满足以下条件的有多少种？

- 从左到右读取红色字符所得到的字符串等于从右到左读取蓝色字符所得到的字符串。

## 约束条件

- $1 \leq N \leq 18$
- $S$ 的长度为 $2N$。
- $S$ 由小写英文字母组成。

## 输入

输入从标准输入给出，格式如下：

> $N$
> 
> $S$

## 输出

打印满足条件的字符串着色方式的数量。

```input1
4
cabaacba
```

```output1
4
```

有四种方式可以着色字符串，如下所示：

- cabaacba
- cabaacba
- cabaacba
- cabaacba

```input2
11
mippiisssisssiipsspiim
```

```output2
504
```

```input3
4
abcdefgh
```

```output3
0
```

```input4
18
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

```output4
9075135300
```

答案可能无法用 $32$ 位整数表示。
