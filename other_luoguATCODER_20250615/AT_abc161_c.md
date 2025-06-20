# AT_abc161_c [ABC161C] Replacing Integer

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc161/tasks/abc161_c

青木君は任意の整数 $ x $ に対し、以下の操作を行うことができます。

操作: $ x $ を $ x $ と $ K $ の差の絶対値で置き換える。

整数 $ N $ の初期値が与えられます。この整数に上記の操作を $ 0 $ 回以上好きな回数行った時にとりうる $ N $ の最小値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式

操作を $ 0 $ 回以上好きな回数行った時にとりうる $ N $ の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
7 4
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
2 6
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
1000000000000000000 1
```

### 输出 #3

```
0
```

## 说明/提示

### 制約

- $ 0\ <\ =\ N\ <\ =\ 10^{18} $
- $ 1\ <\ =\ K\ <\ =\ 10^{18} $
- 入力は全て整数

### Sample Explanation 1

最初、 $ N=7 $ です。 $ 1 $ 回操作を行うと、$ N $ は $ |7-4|\ =\ 3 $ となります。 $ 2 $ 回操作を行うと、$ N $ は $ |3-4|=1 $ となり、これが最小です。

### Sample Explanation 2

$ 1 $ 回も操作を行わなかった場合の $ N=2 $ が最小です。