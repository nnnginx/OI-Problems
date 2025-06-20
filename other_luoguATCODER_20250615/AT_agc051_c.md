# AT_agc051_c [AGC051C] Flipper

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc051/tasks/agc051_c

$ 10^9\ \times\ 10^9 $ 個のマスが正方形状に並んでおり、$ (1,\ 1) $ から $ (10^9,\ 10^9) $ までの番号が振られています。 マス $ (i,\ j) $ は上から $ i $ 列目、左から $ j $ 列目のマスです。 はじめ、$ N $ マス $ (x_1,\ y_1),\ \ldots,\ (x_N,\ y_N) $ が黒で、他の全てのマスは白です。

すぬけ君は、以下の操作を何度でも行うことができます。

- 整数 $ x\ (1\ \leq\ x\ \leq\ 10^9\ -\ 1) $ と整数 $ y\ (1\ \leq\ y\ \leq\ 10^9\ -\ 2) $ を選び、$ 6 $ マス $ (x,\ y),\ (x,\ y+1),\ (x,\ y+2),\ (x+1,\ y),\ (x+1,\ y+1),\ (x+1,\ y+2) $ の色を反転させる (黒は白に、白は黒になる)

操作を済ませた後の黒マスの数として考えられる最小のものを計算してください。

## 输入格式

入力は標準入力から以下の形式で与えられる。

> $ N $ $ x_1\ y_1 $ $ : $ $ x_N\ y_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
9
1 2
1 3
2 1
2 3
2 4
3 2
3 3
3 4
4 2
```

### 输出 #1

```
3
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ x_i,\ y_i\ \leq\ 10^9 $
- $ (x_i,\ y_i) $ は互いに異なる。
- 入力中の全ての値は整数である。

### Sample Explanation 1

以下の図で、上から $ i $ 個目の文字列の $ j $ 文字目がマス $ (i,\ j) $ を表します。`#` が黒、`.` が白です。 ``` .##. #.## .### .#.. -&gt; #... .#.# .### .#.. -&gt; #... ..#. .... .#.. ```