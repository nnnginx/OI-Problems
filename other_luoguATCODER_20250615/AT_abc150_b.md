# AT_abc150_b [ABC150B] Count ABC

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc150/tasks/abc150_b

英大文字のみからなる長さ $ N $ の文字列 $ S $ があります。

$ S $ の連続する部分列 (入出力例をご覧ください) として `ABC` がいくつ含まれるかを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式

$ S $ が連続する部分列として含む `ABC` の個数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
10
ZABCDBABCQ
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
19
THREEONEFOURONEFIVE
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
33
ABCCABCBABCCABACBCBBABCBCBCBCABCB
```

### 输出 #3

```
5
```

## 说明/提示

### 制約

- $ 3\ \leq\ N\ \leq\ 50 $
- $ S $ は英大文字のみからなる。

### Sample Explanation 1

$ S $ の $ 2 $ 文字目から $ 4 $ 文字目、および $ 7 $ 文字目から $ 9 $ 文字目の $ 2 $ 箇所の連続する部分列が `ABC` に一致しています。

### Sample Explanation 2

$ S $ は `ABC` に一致する連続する部分列を含みません。