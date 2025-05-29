## 题目描述

Farmer John usually brands his cows with a circular mark, but his branding iron is broken, so he instead must settle for branding each cow with a mark in the shape of a parenthesis ——```(```. He has two breeds of cows on his farm: Holsteins and Guernseys. He brands each of his cows with a parenthesis-shaped mark. Depending on which direction the cow is facing, this might look like either a left parenthesis or a right parenthesis.

FJ's  $ n $  cows are all standing in a row, each facing an arbitrary direction, so the marks on the cows look like a string of parentheses of length  $ n $ . Looking at this lineup, FJ sees a remarkable pattern: if he scans from left to right through just the Holsteins (in the order they appear in the sequence), this gives a balanced string of parentheses; moreover, the same is true for the Guernseys! To see if this is truly a rare event, please help FJ compute the number of possible ways he could assign breeds to his $n$ cows so that this property holds.

There are several ways to define what it means for a string of parentheses to be "balanced". Perhaps the simplest definition is that there must be the same total number of ```(``` and ```)```, and for any prefix of the string, there must be at least as many ```(``` as ```)```. For example, following strings are all balanced:

```
()
(())
()(()())
```

while these are not:

```
)(
())(
((())))
```

题目大意：给定一个长度为 $ n $ 的括号序列，每个要么是```(```，要么是```)```。你可以把每个位置的括号编号为 $ H $ ，或者是编号为 $ G $ ，要求编号后的括号序列所有编号为 $ H $ 的括号连在一起是合法的，所有编号为 $ G $ 的括号连在一起也是合法
的。

其中：
① ```()```是合法的；
② 若 $ A $ 是合法的，则 $ (A) $ 是合法的；
③ 若 $ A,B $ 都是合法的，则 $ AB $ 是合法的。
那么不同的编号方式有多少种？答案对 $ 2012 $ 取模。

## 输入格式

一个长度为 $ n $ 的括号序列。

## 输出格式

不同的编号方式对 $ 2012 $ 取模后的值。

## 样例输入

```
(())
```

## 样例输出

```
6
```

## 提示

```
(())
HHHH
(())
GGGG
(())
HGGH
(())
GHHG
(())
HGHG
(())
GHGH
```

## 数据规模与约定

对于 $100\%$ 的数据满足： $ 1 \leq n \leq 1\times 10^3 $ 。

## 题目来源

Silver

