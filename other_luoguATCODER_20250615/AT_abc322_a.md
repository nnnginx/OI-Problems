# AT_abc322_a [ABC322A] First ABC 2

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc322/tasks/abc322_a

`A`, `B`, `C` からなる長さ $ N $ の文字列 $ S $ が与えられます。  
$ S $ の中で `ABC` が(連続な)部分文字列として初めて現れる位置を答えてください。すなわち、以下の条件を全て満たす整数 $ n $ のうち最小のものを答えてください。

- $ 1\ \leq\ n\ \leq\ N\ -\ 2 $
- $ S $ の $ n $ 文字目から $ n+2 $ 文字目までを取り出して出来る文字列は `ABC` である。

ただし、`ABC` が $ S $ に現れない場合は `-1` を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式

$ S $ の中で `ABC` が部分文字列として初めて現れる位置を出力せよ。ただし、`ABC` が $ S $ に現れない場合は `-1` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
8
ABABCABC
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
3
ACB
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
20
BBAAABBACAACABCBABAB
```

### 输出 #3

```
13
```

## 说明/提示

### 制約

- $ 3\ \leq\ N\ \leq\ 100 $
- $ S $ は `A`, `B`, `C` からなる長さ $ N $ の文字列

### Sample Explanation 1

$ S $ の中で `ABC` が初めて現れるのは $ 3 $ 文字目から $ 5 $ 文字目までの位置です。よって $ 3 $ が答えになります。

### Sample Explanation 2

`ABC` が $ S $ に現れない場合は $ -1 $ を出力してください。