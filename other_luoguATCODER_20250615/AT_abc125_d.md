# AT_abc125_d [ABC125D] Flipping Signs

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc125/tasks/abc125_d

$ N $ 個の整数が並んでおり、順に $ A_1,\ A_2,\ ...,\ A_N $ です。

あなたはこの整数列に対して次の操作を好きなだけ行うことができます。

**操作**: $ 1\ \leq\ i\ \leq\ N-1 $ を満たす整数 $ i $ を選ぶ。$ A_i $ と $ A_{i+1} $ に $ -1 $ を乗算する。

操作終了後の整数列を $ B_1,\ B_2,\ ...,\ B_N $ とします。

$ B_1\ +\ B_2\ +\ ...\ +\ B_N $ の最大値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ ... $ $ A_N $

## 输出格式

$ B_1\ +\ B_2\ +\ ...\ +\ B_N $ の最大値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
-10 5 -4
```

### 输出 #1

```
19
```

## 输入输出样例 #2

### 输入 #2

```
5
10 -4 -8 -11 3
```

### 输出 #2

```
30
```

## 输入输出样例 #3

### 输入 #3

```
11
-1000000000 1000000000 -1000000000 1000000000 -1000000000 0 1000000000 -1000000000 1000000000 -1000000000 1000000000
```

### 输出 #3

```
10000000000
```

## 说明/提示

### 制約

- 入力は全て整数である。
- $ 2\ \leq\ N\ \leq\ 10^5 $
- $ -10^9\ \leq\ A_i\ \leq\ 10^9 $

### Sample Explanation 1

次のように操作を行うと、$ B_1\ =\ 10,\ B_2\ =\ 5,\ B_3\ =\ 4 $ になり、このときの $ B_1\ +\ B_2\ +\ B_3\ =\ 10\ +\ 5\ +\ 4\ =\ 19 $ が最大です。 - $ i $ として $ 1 $ を選ぶ。操作により、整数列は $ 10,\ -5,\ -4 $ に変化する。 - $ i $ として $ 2 $ を選ぶ。操作により、整数列は $ 10,\ 5,\ 4 $ に変化する。

### Sample Explanation 3

出力が $ 32 $ ビット整数型に収まらない場合があります。