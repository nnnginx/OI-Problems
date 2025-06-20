# AT_abc177_b [ABC177B] Substring

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc177/tasks/abc177_b

$ 2 $ つの文字列 $ S $, $ T $ が与えられます。

$ T $ が $ S $ の部分文字列となるように、$ S $ のいくつかの文字を書き換えます。

少なくとも何文字書き換える必要がありますか？

ただし、部分文字列とは連続する部分列のことを指します。例えば、`xxx` は `yxxxy` の部分文字列ですが、`xxyxx` の部分文字列ではありません。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $ $ T $

## 输出格式

$ S $ を書き換える文字数の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
cabacc
abc
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
codeforces
atcoder
```

### 输出 #2

```
6
```

## 说明/提示

### 制約

- $ S,T $ は $ 1 $ 文字以上 $ 1000 $ 文字以下
- $ T $ の長さは $ S $ の長さ以下
- $ S,T $ は 英小文字のみを含む

### Sample Explanation 1

例えば $ S $ の $ 4 $ 文字目の a を c に書き換えることで、$ S $ の $ 2 $～$ 4 $ 文字目が $ T $ と一致します。 $ S $ 自身は $ T $ を部分文字列に持たないので、この $ 1 $ 文字を書き換えるのが最小です。