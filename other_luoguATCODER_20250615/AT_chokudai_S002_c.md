# AT_chokudai_S002_c 和の最大値 α

## 题目描述

[problemUrl]: https://atcoder.jp/contests/chokudai_S002/tasks/chokudai_S002_c

整数のペアが $ N $ 組あります。$ i $ 番目の整数のペアは $ (A_i,\ B_i) $ です。

各ペアについて $ 2 $ つの整数の和を求め、それらのうちの最大値を答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ : $ $ A_N $ $ B_N $

## 输出格式

$ A_i\ +\ B_i $ の最大値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
4 4
3 7
8 1
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
2
12345678 111111111
103050709 20406080
```

### 输出 #2

```
123456789
```

## 说明/提示

### 制約

入力は以下の条件を満たす。

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i,B_i\ \leq\ 10^9 $
- 入力される値は全て整数

### Sample Explanation 1

各ペアの $ 2 $ つの整数の和は以下の通りです。 - $ 1 $ 番目のペア： $ 4+4\ =\ 8 $ - $ 2 $ 番目のペア： $ 3+7\ =\ 10 $ - $ 3 $ 番目のペア： $ 8+1\ =\ 9 $ このうちの最大値は $ 10 $ なので、$ 10 $ を出力します。

### Sample Explanation 2

和はいずれペアでも $ 123456789 $ になります。