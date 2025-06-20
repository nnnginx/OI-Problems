# AT_abc224_e [ABC224E] Integers on Grid

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc224/tasks/abc224_e

縦 $ H $ 行、横 $ W $ 列のマス目があります。上から $ i $ 行目、左から $ j $ 列目のマスをマス $ (i,\ j) $ と呼びます。

それぞれのマスには整数が書かれています。 $ i\ =\ 1,\ 2,\ \ldots,\ N $ について、マス $ (r_i,\ c_i) $ には正整数 $ a_i $ が書かれており、それら以外のマスには $ 0 $ が書かれています。

はじめ、マス $ (R,\ C) $ にコマが置かれています。 高橋君は、コマを「いま置かれているマスから別のマスに移動させる」ことを好きな回数だけ行うことができます。 ただし、コマを移動する際には下記の $ 2 $ つの条件をともに満たさなければなりません。

- 移動先のマスに書かれている整数は、移動前のマスに書かれている整数より真に大きい。
- 移動先のマスは移動前のマスと同じ行にある、または、移動先のマスは移動前のマスと同じ列にある。

$ i\ =\ 1,\ 2,\ \ldots,\ N $ のそれぞれについて、$ (R,\ C)\ =\ (r_i,\ c_i) $ の場合に高橋君がコマの移動を行うことができる回数の最大値を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ N $ $ r_1 $ $ c_1 $ $ a_1 $ $ r_2 $ $ c_2 $ $ a_2 $ $ \vdots $ $ r_N $ $ c_N $ $ a_N $

## 输出格式

$ N $ 行出力せよ。 $ i\ =\ 1,\ 2,\ \ldots,\ N $ について、$ i $ 行目には $ (R,\ C)\ =\ (r_i,\ c_i) $ の場合に高橋君がコマの移動を行うことができる回数の最大値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 3 7
1 1 4
1 2 7
2 1 3
2 3 5
3 1 2
3 2 5
3 3 5
```

### 输出 #1

```
1
0
2
0
3
1
0
```

## 输入输出样例 #2

### 输入 #2

```
5 7 20
2 7 8
2 6 4
4 1 9
1 5 4
2 2 7
5 5 2
1 7 2
4 6 6
1 4 1
2 1 10
5 6 9
5 3 3
3 7 9
3 6 3
4 3 4
3 3 10
4 2 1
3 5 4
1 2 6
4 7 9
```

### 输出 #2

```
2
4
1
5
3
6
6
2
7
0
0
4
1
5
3
0
5
2
4
0
```

## 说明/提示

### 制約

- $ 2\ \leq\ H,\ W\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ N\ \leq\ \min(2\ \times\ 10^5,\ HW) $
- $ 1\ \leq\ r_i\ \leq\ H $
- $ 1\ \leq\ c_i\ \leq\ W $
- $ 1\ \leq\ a_i\ \leq\ 10^9 $
- $ i\ \neq\ j\ \Rightarrow\ (r_i,\ c_i)\ \neq\ (r_j,\ c_j) $
- 入力はすべて整数

### Sample Explanation 1

マス目に書かれた整数は下記の通りです。 ``` 4 7 0 3 0 5 2 5 5 ``` - $ (R,\ C)\ =\ (r_1,\ c_1)\ =\ (1,\ 1) $ の場合、$ (1,\ 1)\ \rightarrow\ (1,\ 2) $ と移動すると、コマの移動を $ 1 $ 回行うことができます。 - $ (R,\ C)\ =\ (r_2,\ c_2)\ =\ (1,\ 2) $ の場合、一度もコマの移動を行うことができません。 - $ (R,\ C)\ =\ (r_3,\ c_3)\ =\ (2,\ 1) $ の場合、$ (2,\ 1)\ \rightarrow\ (1,\ 1)\ \rightarrow\ (1,\ 2) $ と移動すると、コマの移動を $ 2 $ 回行うことができます。 - $ (R,\ C)\ =\ (r_4,\ c_4)\ =\ (2,\ 3) $ の場合、一度もコマの移動を行うことができません。 - $ (R,\ C)\ =\ (r_5,\ c_5)\ =\ (3,\ 1) $ の場合、$ (3,\ 1)\ \rightarrow\ (2,\ 1)\ \rightarrow\ (1,\ 1)\ \rightarrow\ (1,\ 2) $ と移動すると、コマの移動を $ 3 $ 回行うことができます。 - $ (R,\ C)\ =\ (r_6,\ c_6)\ =\ (3,\ 2) $ の場合、$ (3,\ 2)\ \rightarrow\ (1,\ 2) $ と移動すると、コマの移動を $ 1 $ 回行うことができます。 - $ (R,\ C)\ =\ (r_7,\ c_7)\ =\ (3,\ 3) $ の場合、一度もコマの移動を行うことができません。