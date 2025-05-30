得分 : $1600$ 分

## 问题陈述

给定一个长度为 $2N$ 的字符串 $S$，包含 $N$ 次 `a` 和 $N$ 次 `b`。

你将选择字符串 $S$ 中的一些字符。在这里，对于每个 $i = 1,2,...,N$，不允许仅选择以下两个中的一个：第 $i$ 次出现的 `a` 和第 $i$ 次出现的 `b`。 （也就是说，你只能选择两个都选择，或者都不选择。）然后，你将按顺序连接所选择的字符。

找出通过这种方式可以得到的字典序最大的字符串。

## 约束条件

- $1 \leq N \leq 3000$
- $S$ 是一个长度为 $2N$ 的字符串，包含 $N$ 次 `a` 和 $N$ 次 `b`。

## 输入

输入从标准输入给出，格式如下：

> $N$
> 
> $S$

## 输出

打印满足条件的字典序最大的字符串。

```input1
3
aababb
```

```output1
abab
```

从 $S$ 中取第一个、第三个、第四个和第六个字符得到的子序列 $T$ 满足条件。

```input2
3
bbabaa
```

```output2
bbabaa
```

你可以选择所有字符。

```input3
6
bbbaabbabaaa
```

```output3
bbbabaaa
```

```input4
9
abbbaababaababbaba
```

```output4
bbaababababa
```  
