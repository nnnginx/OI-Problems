# AT_diverta2019_2_b Picking Up

## 题目描述

[problemUrl]: https://atcoder.jp/contests/diverta2019-2/tasks/diverta2019_2_b

$ 2 $ 次元平面上に $ N $ 個のボールがあり、$ i $ 番目のボールは $ (x_i,\ y_i) $ にあります。

まず、$ p\ \neq\ 0 $ または $ q\ \neq\ 0 $ を満たす $ 2 $ つの整数 $ p,\ q $ を決め、その後以下の操作を繰り返してボールを全て回収します。

- 残っているボールを $ 1 $ つ選んで回収する。このボールの座標を $ (a,\ b) $ とする。この時、直前に選んだボールの座標が $ (a\ -\ p,\ b\ -\ q) $ である時コスト $ 0 $ 、そうでない時コスト $ 1 $ かかる。ただし、$ 1 $ つ目に選んだボールについては必ずコスト $ 1 $ かかる。

$ p,\ q $ を最適に選んだ場合にボールを全て回収するのにかかるコストの和の最小値を計算してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ x_1 $ $ y_1 $ $ : $ $ x_N $ $ y_N $

## 输出格式

ボールを全て回収するのにかかるコストの和の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2
1 1
2 2
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
3
1 4
4 6
7 8
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
4
1 1
1 2
2 1
2 2
```

### 输出 #3

```
2
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 50 $
- $ |x_i|,\ |y_i|\ \leq\ 10^9 $
- $ x_i\ \neq\ x_j $ または $ y_i\ \neq\ y_j\ (i\ \neq\ j) $
- 入力は全て整数である

### Sample Explanation 1

$ p\ =\ 1,\ q\ =\ 1 $ とすると、$ (1,\ 1) $ のボール、$ (2,\ 2) $ のボールの順に選ぶことでコスト $ 1 $ でボールを全て回収することができます。

### Sample Explanation 2

$ p\ =\ -3,\ q\ =\ -2 $ とすると、$ (7,\ 8) $ のボール、$ (4,\ 6) $ のボール、$ (1,\ 4) $ のボールの順に選ぶことでコスト $ 1 $ でボールを全て回収することができます。