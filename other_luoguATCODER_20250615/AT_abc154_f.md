# AT_abc154_f [ABC154F] Many Many Paths

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc154/tasks/abc154_f

$ 2 $ 次元平面があります。この平面上に立っているすぬけ君は、一回の操作で $ x $ 軸正の方向に $ 1 $ もしくは $ y $ 軸正の方向に $ 1 $ 移動することができます。

また、以下のように関数 $ f(r,c) $ を定義します。

- $ f(r,c)\ := $ (すぬけ君が点 $ (0,0) $ から点 $ (r,c) $ まで上記の操作を繰り返して到達する経路の個数)

整数 $ r_1,\ r_2,\ c_1,\ c_2 $ が与えられます。 $ r_1\ <\ =\ i\ <\ =\ r_2 $ かつ $ c_1\ <\ =\ j\ <\ =\ c_2 $ を満たす全ての整数の組 $ (i,j) $ に対する $ f(i,j) $ の 総和を求め、 $ (10^9+7) $ で割った余りを計算してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ r_1 $ $ c_1 $ $ r_2 $ $ c_2 $

## 输出格式

$ f(i,j) $ の総和を $ (10^9+7) $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1 1 2 2
```

### 输出 #1

```
14
```

## 输入输出样例 #2

### 输入 #2

```
314 159 2653 589
```

### 输出 #2

```
602215194
```

## 说明/提示

### 制約

- $ 1\ <\ =\ r_1\ <\ =\ r_2\ <\ =\ 10^6 $
- $ 1\ <\ =\ c_1\ <\ =\ c_2\ <\ =\ 10^6 $
- 入力はすべて整数

### Sample Explanation 1

例えば、点 $ (0,0) $ から点 $ (1,1) $ までの経路は、$ (0,0) $ → $ (0,1) $ → $ (1,1) $ と $ (0,0) $ → $ (1,0) $ → $ (1,1) $ の $ 2 $ 通りあるので、 $ f(1,1)=2 $ です。 同様に、$ f(1,2)=3 $, $ f(2,1)=3 $, $ f(2,2)=6 $ なので、求める総和は $ 14 $ です。