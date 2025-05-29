## 题目描述

给定一个由小写字符构成的字符串 $S$。

令一个字符串串的价值为该串的**本质不同**非空子序列个数，其中子序列可以为整体。

求 $S$ 所有子序列的价值和。答案对 $10^9+7$ 取模。

## 输入格式

第一行一个由小写字符构成的字符串 $S$。

## 输出格式

输出一行，为答案。

```input1
ab
```
```output1
5
```

```input2
sapnap
```
```output2
593
```

```input3
abcbdabcbabcd
```
```output3
938773
```

```input4
tobeornottobethatisthequestion
```
```output4
769276982
```

## 数据规模与约定

**本题采用捆绑测试。**

 - Subtask 1（5 pts）：$|S|\le 11$。
 - Subtask 2（10 pts）：$|S|\le 22$。
 - Subtask 3（20 pts）：$|S|\le 100$ 并 $S$ 仅由 `a`，`b` 两个字符构成。
 - Subtask 4（30 pts）：$|S|\le 5000$。
 - Subtask 5（35 pts）：无特殊限制。

对于 $100\%$ 的数据，$1\le |S|\le 10^6$，保证 $S$ 仅由小写字符构成。