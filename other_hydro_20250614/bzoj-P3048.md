## 题目描述

Farmer John's  $ n $  cows are lined up in a row. Each cow is identified by an integer "breed ID" in the range  $ 0...1\times 10^9 $ ; the breed ID of the ith cow in the lineup is  $ B(i) $ . Multiple cows can share the same breed ID. FJ thinks that his line of cows will look much more impressive if there is a large contiguous block of cows that all have thesame breed ID. In order to create such a block, FJ chooses up to K breed IDs and removes from his lineup all the cows having those IDs. Please help FJ figure out the length of the largest consecutive block of cows with the same breed ID that he can create by doing this.

给你一个长度为 $ n $ 的自然数数列，其中每一个数都小于等于 $ 1\times 10^9 $，现在给你一个 $ k $，表示你最多可以删去 $ k $ 类数。数列中相同的数字被称为一类数。设该数列中满足所有的数字相等的连续子序列被叫做完美序列，你的任务就是通过删数使得该数列中的最长完美序列尽量长。

## 输入格式

Line 1: Two space-separated integers:  $ n $  and  $ k $.
Lines 2..1+N: Line i+1 contains the breed ID $ B(i) $.

## 输出格式

Line 1: The largest size of a contiguous block of cows with identical breed IDs that FJ can create.

## 样例输入

```
9 1
2
7
3
7
7
3
7
5
7
```

## 样例输出

```
4
```

## 提示

长度为9的数列，最多只能删去 $ 1 $ 类数。

不删，最长完美序列长度为 $ 2 $ 。

删去一类数 $ 3 $ ，序列变成 $ 2,7,7,7,7,5,7 $ ，最长完美序列长度为 $ 4 $ .因此答案为 $ 4 $ .

## 数据规模与约定

对于 $100\%$ 的数据，$  1 \leq n \leq 1\times 10^5  $。

## 题目来源

Gold

