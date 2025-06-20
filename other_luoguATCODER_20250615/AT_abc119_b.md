# AT_abc119_b [ABC119B] Digital Gifts

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc119/tasks/abc119_b

高橋くんは $ N $ 人の親戚からお年玉をもらいました。

$ N $ 個の値 $ x_1,\ x_2,\ ...,\ x_N $ と $ N $ 個の文字列 $ u_1,\ u_2,\ ...,\ u_N $ が入力されます。各文字列 $ u_i $ は `JPY` または `BTC` であり、$ x_i $ と $ u_i $ が $ i $ 人目の親戚からのお年玉の内容を表します。

例えば、$ x_1\ = $ `10000`, $ u_1\ = $ `JPY` であれば $ 1 $ 人目の親戚からのお年玉は $ 10000 $ 円であり、$ x_2\ = $ `0.10000000`, $ u_2\ = $ `BTC` であれば $ 2 $ 人目の親戚からのお年玉は $ 0.1 $ ビットコインです。

ビットコインを $ 1.0 $ BTC あたり $ 380000.0 $ 円として換算すると、高橋くんがもらったお年玉は合計で何円に相当するでしょうか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ x_1 $ $ u_1 $ $ x_2 $ $ u_2 $ $ : $ $ x_N $ $ u_N $

## 输出格式

高橋くんが受け取ったお年玉が合計で $ Y $ 円に相当するとき、値 $ Y $ (整数とは限らない) を出力せよ。

出力は、ジャッジの出力との絶対誤差または相対誤差が $ 10^{-5} $ 以下のとき正解と判定される。

## 输入输出样例 #1

### 输入 #1

```
2
10000 JPY
0.10000000 BTC
```

### 输出 #1

```
48000.0
```

## 输入输出样例 #2

### 输入 #2

```
3
100000000 JPY
100.00000000 BTC
0.00000001 BTC
```

### 输出 #2

```
138000000.0038
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 10 $
- $ u_i\ = $ `JPY` または `BTC`
- $ u_i\ = $ `JPY` のとき $ x_i $ は整数であり、$ 1\ \leq\ x_i\ \leq\ 10^8 $
- $ u_i\ = $ `BTC` のとき $ x_i $ は小数点以下の桁を $ 8 $ 桁持つ小数であり、$ 0.00000001\ \leq\ x_i\ \leq\ 100.00000000 $

### Sample Explanation 1

$ 1 $ 人目の親戚からのお年玉は $ 10000 $ 円です。$ 2 $ 人目の親戚からのお年玉は $ 0.1 $ ビットコインであり、$ 1 $ BTC あたり $ 380000.0 $ 円として換算すると $ 38000.0 $ 円となります。これらの合計は $ 48000.0 $ 円です。 なお、`48000`、`48000.1` などと出力しても正解と判定されます。

### Sample Explanation 2

この場合、`138001000`、`1.38e8` などと出力しても正解と判定されます。