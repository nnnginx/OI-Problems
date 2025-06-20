# AT_bcu30_d 数直線

## 题目描述

[problemUrl]: https://atcoder.jp/contests/bcu30/tasks/bcu30_d

数直線上に $ N $ 個の点があります。 $ i $ 番目 $ (1\ \leq\ i\ \leq\ N) $ の点の座標は $ x_i $ です。

また、座標 $ p $ と座標 $ q $ の距離は $ |p-q| $ です。

$ Q $ 個のクエリが与えられます。 $ i $ 番目 $ (1\ \leq\ i\ \leq\ Q) $ のクエリでは、数直線上の座標 $ t_i $ が与えられます。 この点から $ N $ 個の点への距離の総和を求めてください。

## 输入格式

入力は以下の形式で与えられる。

> $ N $ $ Q $ $ x_1 $ ... $ x_N $ $ t_1 $ : $ t_Q $

## 输出格式

$ i $ 行目 $ (1\ \leq\ i\ \leq\ Q) $ に $ i $ 番目のクエリの答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 4
1 4 5 8 10
3
4
7
11
```

### 输出 #1

```
17
14
15
27
```

## 输入输出样例 #2

### 输入 #2

```
8 10
-499 -120 32 255 571 890 1011 1256
0
-200
2500
364
-117
50
-612
889
32
364
```

### 输出 #2

```
4634
5594
16604
4060
5102
4470
8292
4696
4506
4060
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100,000 $
- $ 1\ \leq\ Q\ \leq\ 100,000 $
- $ -10^9\ \leq\ x_i\ \leq\ 10^9 $ $ (1\ \leq\ i\ \leq\ N) $
- $ -10^9\ \leq\ t_i\ \leq\ 10^9 $ $ (1\ \leq\ i\ \leq\ Q) $
- $ x_i\ <\ x_{i+1} $ $ (1\ \leq\ i\ \leq\ N-1) $

### Sample Explanation 1

たとえば、$ 1 $ 番目のクエリでは $ t_1=3 $ が与えられます。この座標から $ N $ 個の点への距離の総和は、 $ |1-3|\ +\ |4-3|\ +\ |5-3|\ +\ |8-3|\ +\ |10-3|\ =\ 17 $ となります。