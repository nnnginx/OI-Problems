# AT_icpc2016autumn_a Best Matched Pair

## 题目描述

给定 $n(1\le n\le 1000)$ 个互不相同的正整数 $a_i(1\le a_i\le10^4)$。现在求 $a_i\times a_j(i\ne j)$ 的最大值。

这个乘积需要保证从高到低的对应数字依次递增且连续，如：$1234$ 是合法的，$4321$ 与 $1245$ 都是不合法的。

## 输入格式

第一行一个正整数 $n$。

接下来一行共 $n$ 个正整数 $a_i$。

## 输出格式

输出最大的符合要求的乘积。如果没有，输出 `-1`。

**特别的，对于本题，您应该在行末输出一个换行，否则评测机会返回 `WA`。**

## 输入输出样例 #1

### 输入 #1

```
2
1 2
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
3
3 22 115
```

### 输出 #2

```
345
```

## 输入输出样例 #3

### 输入 #3

```
2
1 11
```

### 输出 #3

```
-1
```

## 输入输出样例 #4

### 输入 #4

```
2
5 27
```

### 输出 #4

```
-1
```

## 输入输出样例 #5

### 输入 #5

```
2
17 53
```

### 输出 #5

```
-1
```

## 输入输出样例 #6

### 输入 #6

```
10
53 43 36 96 99 2 27 86 93 23
```

### 输出 #6

```
3456
```

## 说明/提示

Translate by @[tianbiandeshenghuo11](/user/752485)