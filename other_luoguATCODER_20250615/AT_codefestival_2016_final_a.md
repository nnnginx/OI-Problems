# AT_codefestival_2016_final_a Where&#39;s Snuke?

## 题目描述

[problemUrl]: https://atcoder.jp/contests/cf16-final/tasks/codefestival_2016_final_a

縦 $ H $ 行、横 $ W $ 列のマス目があります。

上から $ i $ 行目、左から $ j $ 列目には長さ $ 5 $ の文字列 $ S_{i,j} $ が書かれています。

行には上から順に $ 1 $~$ H $ の番号が、列には左から順に `A`~`Z` の番号がついています。

![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_codefestival_2016_final_a/d3b854eace34ecfd0d0564d0ea4b3c7c5a522480.png)

この中から `snuke` という文字列を探し、列と行の番号を順に続けて出力してください。

例えば $ 6 $ 行目の $ 8 $ 列目にあった場合は、`H6` のように出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ S_{1,1} $ $ S_{1,2} $ $ ... $ $ S_{1,W} $ $ S_{2,1} $ $ S_{2,2} $ $ ... $ $ S_{2,W} $ $ : $ $ S_{H,1} $ $ S_{H,2} $ $ ... $ $ S_{H,W} $

## 输出格式

`snuke` という文字列が書かれているマスの列と行の番号を続けて出力せよ。

## 输入输出样例 #1

### 输入 #1

```
15 10
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snuke snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
snake snake snake snake snake snake snake snake snake snake
```

### 输出 #1

```
H6
```

## 输入输出样例 #2

### 输入 #2

```
1 1
snuke
```

### 输出 #2

```
A1
```

## 说明/提示

### 制約

- $ 1≦H,\ W≦26 $
- $ S_{i,j} $ は小文字アルファベット（`a`-`z`）のみからなる長さ $ 5 $ の文字列である。
- 与えられる文字列のうち、ちょうど $ 1 $ つだけが `snuke` である。