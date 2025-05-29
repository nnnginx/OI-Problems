## 题目描述

给出一个由小写字母组成的字符串 $s$，问有多少由小写字母构成的字条串 $s'$ ，满足：

1. $ |s|'=|s|$；
2. $s'[l\dots r]$ 是回文串，当且仅当 $s[l\dots r]$ 是回文串。

## 输入格式

一个字符串 $s$。

## 输出格式

输出答案 $\mod 10^9+7$。

```input1
abba
```

```output1
650
```

## 样例说明

Only words of the form `xyyx` are palindromically equivalent to `abba`, where `x` and `y` are distinct letters.
The English alphabet contains $26$ letters, consequently there are $26\times25=650$ such words in total.

## 数据规模与约定

对于 $100\%$ 的数据，$s$ 长度 $\le 10^6$。

