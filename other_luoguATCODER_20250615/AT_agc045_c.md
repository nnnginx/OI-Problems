# AT_agc045_c [AGC045C] Range Set

## 题目描述

Snuke 君有长为 $N$ 的字符串 $x$，最初 $x$ 的所有字符都是 $0$。Snuke 君可以按照任意顺序进行任意次数以下两种操作:

- 选择 $x$ 中连续的长为 $A$ 的子串，将它们全部设为 $0$。
- 选择 $x$ 中连续的长为 $B$ 的子串，将它们全部设为 $1$。

请计算操作结束后的可能达成的不同的 $x$ 的数量，对 $10^9+7$ 取模。

## 输入格式

一行三个整数 $N$，$A$，$B$。

## 输出格式

一行一个整数，表示你的答案。

## 输入输出样例 #1

### 输入 #1

```
4 2 3
```

### 输出 #1

```
11
```

## 输入输出样例 #2

### 输入 #2

```
10 7 2
```

### 输出 #2

```
533
```

## 输入输出样例 #3

### 输入 #3

```
1000 100 10
```

### 输出 #3

```
828178524
```