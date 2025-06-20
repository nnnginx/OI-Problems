# AT_nikkei2019_qual_b Touitsu

## 题目描述

[problemUrl]: https://atcoder.jp/contests/nikkei2019-qual/tasks/nikkei2019_qual_b

三つの文字列 $ A,\ B,\ C $ が与えられます。これらはそれぞれ、英小文字からなる長さ $ N $ の文字列です。

私たちの目標は、これら三つの文字列をすべて等しくすることです。そのために、あなたは次の操作を繰り返し行うことができます。

- 操作: 文字列 $ A,\ B,\ C $ のうち一つを選び、さらに $ 1 $ 以上 $ N $ 以下の整数 $ i $ を指定する。そして、選んだ文字列の先頭から $ i $ 文字目を別の何らかの英小文字に変更する。

目標を達成するためには最小で何回の操作が必要でしょうか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A $ $ B $ $ C $

## 输出格式

必要な最小の操作回数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
west
east
wait
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
9
different
different
different
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
7
zenkoku
touitsu
program
```

### 输出 #3

```
13
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ A,\ B,\ C $ はそれぞれ長さ $ N $ の文字列である。
- $ A,\ B,\ C $ の各文字は英小文字である。

### Sample Explanation 1

この例では、はじめ $ A\ = $ `west`、$ B\ = $ `east`、$ C\ = $ `wait` です。以下のように $ 3 $ 回の操作を行うことで、最小の操作回数で目標を達成できます。 - $ A $ の $ 2 $ 文字目を `a` に変更する。$ A $ は `wast` となる。 - $ B $ の $ 1 $ 文字目を `w` に変更する。$ B $ は `wast` となる。 - $ C $ の $ 3 $ 文字目を `s` に変更する。$ C $ は `wast` となる。

### Sample Explanation 2

はじめから $ A,\ B,\ C $ がすべて等しい場合、必要な操作回数は $ 0 $ となります。