# AT_abc047_b [ABC047B] すぬけ君の塗り絵 2 イージー

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc047/tasks/abc047_b

$ xy $ 平面上に、左下の座標が $ (0,\ 0) $、右上の座標が $ (W,\ H) $ で、各辺が $ x $ 軸か $ y $ 軸に平行な長方形があります。最初、長方形の内部は白く塗られています。

すぬけ君はこの長方形の中に $ N $ 個の点を打ちました。$ i $ 個目 ($ 1\ ≦\ i\ ≦\ N $) 点の座標は $ (x_i,\ y_i) $ でした。

また、すぬけ君は長さ $ N $ の数列 $ a $ を決めて、各 $ 1\ ≦\ i\ ≦\ N $ に対し、

- $ a_i\ =\ 1 $ のときは長方形の $ x\ <\ x_i $ をみたす領域
- $ a_i\ =\ 2 $ のときは長方形の $ x\ >\ x_i $ をみたす領域
- $ a_i\ =\ 3 $ のときは長方形の $ y\ <\ y_i $ をみたす領域
- $ a_i\ =\ 4 $ のときは長方形の $ y\ >\ y_i $ をみたす領域

を黒く塗りました。

塗りつぶしが終わったあとの長方形内での白い部分の面積を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ W $ $ H $ $ N $ $ x_1 $ $ y_1 $ $ a_1 $ $ x_2 $ $ y_2 $ $ a_2 $ $ : $ $ x_N $ $ y_N $ $ a_N $

## 输出格式

塗りつぶしが終わったあとの長方形内での白い部分の面積を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 4 2
2 1 1
3 3 4
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
5 4 3
2 1 1
3 3 4
1 4 2
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
10 10 5
1 6 1
4 1 3
6 9 4
9 4 2
3 1 3
```

### 输出 #3

```
64
```

## 说明/提示

### 制約

- $ 1\ ≦\ W,\ H\ ≦\ 100 $
- $ 1\ ≦\ N\ ≦\ 100 $
- $ 0\ ≦\ x_i\ ≦\ W $ ($ 1\ ≦\ i\ ≦\ N $)
- $ 0\ ≦\ y_i\ ≦\ H $ ($ 1\ ≦\ i\ ≦\ N $)
- $ W $, $ H $ (21:32 追記), $ x_i $, $ y_i $ は整数である
- $ a_i $ ($ 1\ ≦\ i\ ≦\ N $) は $ 1,\ 2,\ 3,\ 4 $ のいずれかである

### Sample Explanation 1

すぬけ君が塗りつぶしを始める前の長方形は以下の図のようになっています。 !\[e19e673abcd0882783f635cce9d2f94d.png\](https://atcoder.jp/img/abc047/e19e673abcd0882783f635cce9d2f94d.png) $ (x_1,\ y_1)\ =\ (2,\ 1) $、$ a_1\ =\ 1 $ なので、まずすぬけ君は $ x $ 座標が $ 2 $ より小さい領域を塗りつぶし、長方形は以下のようになります。 !\[f25cd04bbac23c4e5426d70511a9762f.png\](https://atcoder.jp/img/abc047/f25cd04bbac23c4e5426d70511a9762f.png) $ (x_2,\ y_2)\ =\ (3,\ 3) $、$ a_2\ =\ 4 $ なので、次にすぬけ君は $ y $ 座標が $ 3 $ より大きい領域を塗りつぶし、長方形は最終的に以下のようになります。 !\[46b0c06fd9eee4f148e1f441f7abca53.png\](https://atcoder.jp/img/abc047/46b0c06fd9eee4f148e1f441f7abca53.png) この最終的な状態における白い部分の面積は $ 9 $ なので、出力は $ 9 $ となります。

### Sample Explanation 2

塗りつぶした結果、白い部分が残らないこともありえます。