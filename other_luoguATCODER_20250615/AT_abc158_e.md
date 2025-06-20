# AT_abc158_e [ABC158E] Divisible Substring

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc158/tasks/abc158_e

高橋君は `0` から `9` までの数字から成る長さ $ N $ の文字列 $ S $ を持っています。

素数 $ P $ が好きな高橋君は、$ S $ の空でない連続する部分文字列 $ N\ \times\ (N\ +\ 1)\ /\ 2 $ 個のうち、十進表記の整数と見なした際に $ P $ で割り切れるものの個数を知りたくなりました。

ただし部分文字列は先頭が `0` であっても良いものとし、文字列として等しい場合や、整数と見なした際に等しい場合も、部分文字列の $ S $ 内の位置で区別します。

高橋君のためにこの個数を計算してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ P $ $ S $

## 输出格式

$ S $ の空でない連続する部分文字列であって、十進表記の整数と見なした際に $ P $ で割り切れるものの個数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 3
3543
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
4 2
2020
```

### 输出 #2

```
10
```

## 输入输出样例 #3

### 输入 #3

```
20 11
33883322005544116655
```

### 输出 #3

```
68
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ S $ は数字から成る
- $ |S|\ =\ N $
- $ 2\ \leq\ P\ \leq\ 10000 $
- $ P $ は素数である

### Sample Explanation 1

$ S $ = `3543` です。$ S $ の空でない連続する部分文字列は次の $ 10 $ 個があります。 - `3` は $ 3 $ で割り切れる。 - `35` は $ 3 $ で割り切れない。 - `354` は $ 3 $ で割り切れる。 - `3543` は $ 3 $ で割り切れる。 - `5` は $ 3 $ で割り切れない。 - `54` は $ 3 $ で割り切れる。 - `543` は $ 3 $ で割り切れる。 - `4` は $ 3 $ で割り切れない。 - `43` は $ 3 $ で割り切れない。 - `3` は $ 3 $ で割り切れる。 このうち $ 3 $ で割り切れるものは $ 6 $ 個であるので、$ 6 $ を出力してください。

### Sample Explanation 2

$ S $ = `2020` です。$ S $ の空でない連続する部分文字列は $ 10 $ 個ありますが、その全てが $ 2 $ で割り切れるので $ 10 $ を出力してください。 先頭が `0` である部分文字列も許容されることに注意してください。