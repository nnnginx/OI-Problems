# AT_jag2018summer_day2_h Prefix Suffix Free

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jag2018summer-day2/tasks/jag2018summer_day2_h

You are given a string $ S $ consisting of lowercase English letters. Count the number of strings $ T $ that satisfies all of the following conditions:

- $ T $ is a string of the same length as $ S $, consisting of lowercase English letters.
- For all $ K $ ( $ 1\ \leq\ K\ \leq\ |S| $ ), the string formed by the first $ K $ letters of $ S $ does not coincide with the string formed by the last $ K $ letters of $ T $.

Since the answer can be very large, find the number modulo $ 10^9+7 $.

## 输入格式

Input is given from Standard Input in the following format:

> $ S $

## 输出格式

Print the number of strings that satisfy the condition, modulo $ 10^9+7 $.

## 输入输出样例 #1

### 输入 #1

```
aa
```

### 输出 #1

```
650
```

## 输入输出样例 #2

### 输入 #2

```
abc
```

### 输出 #2

```
16873
```

## 输入输出样例 #3

### 输入 #3

```
xrxbaxrxikxrxgvcpuwx
```

### 输出 #3

```
352084595
```

## 说明/提示

### Constraints

- $ 1\ \leq\ |S|\ \leq\ 10^6 $
- $ S $ consists of lowercase English letters.

### Sample Explanation 1

For example, $ T= $ `zz` and `ab` satisfy the condition, but `ba` or `aa` does not.