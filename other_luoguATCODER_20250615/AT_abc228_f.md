# AT_abc228_f [ABC228F] Stamp Game

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc228/tasks/abc228_f

縦 $ H $ 行、横 $ W $ 列のマス目があります。上から $ i $ 行目、左から $ j $ 列目のマスをマス $ (i,\ j) $ と呼びます。  
 $ 1\ \leq\ i\ \leq\ H $ かつ $ 1\ \leq\ j\ \leq\ W $ を満たす整数の組 $ (i,\ j) $ それぞれについて、マス $ (i,\ j) $ には正整数 $ A_{i,\ j} $ が書かれています。また、すべてのマスは白色に塗られています。

高橋君は、縦 $ h_1 $ 行、横 $ w_1 $ 列の長方形の黒いスタンプを持っており、青木君は、縦 $ h_2 $ 行、横 $ w_2 $ 列の長方形の白いスタンプを持っています。  
 $ 2 $ 人はこれらのスタンプとマス目を使って対戦ゲームをします。

まず高橋君が、持っている黒いスタンプを $ 1 $ 回使って、マス目の縦 $ h_1 $ 行、横 $ w_1 $ 列の長方形領域を黒色に塗りつぶします。  
 すなわち、$ 1\ \leq\ i\ \leq\ H\ -\ h_1\ +\ 1 $ かつ $ 1\ \leq\ j\ \leq\ W\ -\ w_1\ +\ 1 $ を満たす整数の組 $ (i,\ j) $ を一つ選び、 $ i\ \leq\ r\ \leq\ i\ +\ h_1\ -\ 1 $ かつ $ j\ \leq\ c\ \leq\ j\ +\ w_1\ -\ 1 $ を満たすすべてのマス $ (r,\ c) $ を黒色に塗りつぶします。

次に青木君が、持っている白いスタンプを $ 1 $ 回使って、マス目の縦 $ h_2 $ 行、横 $ w_2 $ 列の長方形領域を白色に塗りつぶします。  
 すなわち、$ 1\ \leq\ i\ \leq\ H\ -\ h_2\ +\ 1 $ かつ $ 1\ \leq\ j\ \leq\ W\ -\ w_2\ +\ 1 $ を満たす整数の組 $ (i,\ j) $ を一つ選び、 $ i\ \leq\ r\ \leq\ i\ +\ h_2\ -\ 1 $ かつ $ j\ \leq\ c\ \leq\ j\ +\ w_2\ -\ 1 $ を満たすすべてのマス $ (r,\ c) $ を白色に塗りつぶします。  
 このとき、青木君が白色に塗るマスがすでに高橋君によって黒色に塗られていた場合は、そのマスの色は白で上書きされます。

上記の通りに高橋君と青木君がスタンプを $ 1 $ 回ずつ使った後の、黒色に塗られたマスに書かれた整数の合計を、ゲームの「スコア」とします。 高橋君はスコアが出来るだけ大きくなるように、青木君はスコアが出来るだけ小さくなるように、それぞれ最適な戦略をとります。 ゲームのスコアがいくらになるかを求めて下さい。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ h_1 $ $ w_1 $ $ h_2 $ $ w_2 $ $ A_{1,\ 1} $ $ A_{1,\ 2} $ $ \cdots $ $ A_{1,\ W} $ $ A_{2,\ 1} $ $ A_{2,\ 2} $ $ \cdots $ $ A_{2,\ W} $ $ \vdots $ $ A_{H,\ 1} $ $ A_{H,\ 2} $ $ \cdots $ $ A_{H,\ W} $

## 输出格式

高橋君はスコアが出来るだけ大きくなるように、青木君はスコアが出来るだけ小さくなるように、それぞれ最適な戦略をとるときの、ゲームのスコアを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 4 2 3 3 1
3 1 4 1
5 9 2 6
5 3 5 8
```

### 输出 #1

```
19
```

## 输入输出样例 #2

### 输入 #2

```
3 4 2 3 3 4
3 1 4 1
5 9 2 6
5 3 5 8
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
10 10 3 7 2 3
9 7 19 7 10 4 13 9 4 8
10 15 16 3 18 19 17 12 13 2
12 18 4 9 13 13 6 13 5 2
16 12 2 14 18 17 14 7 8 12
12 13 17 12 14 15 19 7 13 15
5 2 16 10 4 6 1 2 7 8
10 14 14 10 9 13 11 4 9 19
16 12 3 19 19 6 2 19 14 20
15 3 19 19 2 10 1 4 3 15
13 20 5 6 19 1 7 17 10 19
```

### 输出 #3

```
180
```

## 说明/提示

### 制約

- $ 2\ \leq\ H,\ W\ \leq\ 1000 $
- $ 1\ \leq\ h_1,\ h_2\ \leq\ H $
- $ 1\ \leq\ w_1,\ w_2\ \leq\ W $
- $ 1\ \leq\ A_{i,\ j}\ \leq\ 10^9 $
- 入力はすべて整数

### Sample Explanation 1

ゲームは以下の通りに進行します。 - はじめ、すべてのマスは白色で塗られています。 - まず高橋君が、持っている縦 $ 2 $ 行横 $ 3 $ 列の黒いスタンプを使って、マス $ (2,\ 2),\ (2,\ 3),\ (2\ ,4),\ (3,\ 2),\ (3,\ 3),\ (3,\ 4) $ の $ 6 $ つのマスを黒色で塗りつぶします。 - 次に青木君が、持っている縦 $ 3 $ 行横 $ 1 $ 列の白いスタンプを使って、マス $ (1,\ 4),\ (2,\ 4),\ (3,\ 4) $ を白色で塗りつぶします。 - 最終的に黒色で塗られているマスは、マス $ (2,\ 2),\ (2,\ 3),\ (3,\ 2),\ (3,\ 3) $ の $ 4 $ つであるため、ゲームのスコアは $ 9\ +\ 2\ +\ 3\ +\ 5\ =\ 19 $ です。

### Sample Explanation 2

青木君がスタンプを使った後、すべてのマスは白色であり、ゲームのスコアは $ 0 $ となります。