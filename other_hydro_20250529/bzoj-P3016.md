## 题目描述

Bessie the cow is trying to type a balanced string of parentheses into her new laptop, but she is sufficiently clumsy (due to her large hooves) that she keeps mis-typing characters. Please help her by computing the minimum number of characters in the string that one must reverse (e.g., changing a left parenthesis to a right parenthesis, or vice versa) so that the string would become balanced. There are several ways to define what it means for a string of parentheses to be "balanced". Perhaps the simplest definition is that there must be the same total number of ```(``` and ```)```, and for any prefix of the string, there must be at least as many ```(``` as ```)```.

For example, the following strings are all balanced:

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

题目大意：给定长度为 $n$ 的一个括号序列，每次修改可以修改一个位置的括号，若这个括号为```(```，则修改为```)```，若这个括号为```)```，则修改为```(```，问最少修改多少个使得原括号序列合法。
其中：
① ```()```是合法的；
② 若 $A$ 是合法的，则 $(A)$ 是合法的；
③ 若 $A,B$ 都是合法的，则 $AB$ 是合法的。

## 输入格式

一个长度为 $n$ 个括号序列。

## 输出格式

最少的修改次数。

## 样例输入

```
())(
```

## 样例输出

```
2
```

## 提示

修改为```()()```，其中红色部分表示修改的括号。

## 数据规模与约定

对于 $100\%$ 的数据满足：$1 \leq n \leq 1\times 10^5$。

## 题目来源

Silver

