# AT_arc101_b [ABC107D] Median of Medians

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc107/tasks/arc101_b

長さ $ M $ の数列 $ b $ の **中央値** を次のように定義します。

- $ b $ を昇順にソートして得られる数列を $ b' $ とする。 このとき、$ b' $ の $ M\ /\ 2\ +\ 1 $ 番目の要素の値を、$ b $ の中央値とする。 ここで、$ / $ は小数点以下を切り捨てる除算である。

例えば、$ (10,\ 30,\ 20) $ の中央値は $ 20 $ であり、$ (10,\ 30,\ 20,\ 40) $ の中央値は $ 30 $ であり、$ (10,\ 10,\ 10,\ 20,\ 30) $ の中央値は $ 10 $ です。

すぬけ君は次のような問題を思いつきました。

長さ $ N $ の数列 $ a $ があります。 各 $ (l,\ r) $ ($ 1\ \leq\ l\ \leq\ r\ \leq\ N $) について、$ a $ の連続部分列 $ (a_l,\ a_{l\ +\ 1},\ ...,\ a_r) $ の中央値を $ m_{l,\ r} $ とします。 すべての $ (l,\ r) $ に対する $ m_{l,\ r} $ を並べ、新たに数列 $ m $ を作ります。 $ m $ の中央値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ a_2 $ $ ... $ $ a_N $

## 输出格式

$ m $ の中央値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
10 30 20
```

### 输出 #1

```
30
```

## 输入输出样例 #2

### 输入 #2

```
1
10
```

### 输出 #2

```
10
```

## 输入输出样例 #3

### 输入 #3

```
10
5 9 5 9 8 9 3 5 4 3
```

### 输出 #3

```
8
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ a_i $ は整数である。
- $ 1\ \leq\ a_i\ \leq\ 10^9 $

### Sample Explanation 1

$ a $ のそれぞれの連続部分列の中央値は次のようになります。 - $ (10) $ の中央値は $ 10 $ - $ (30) $ の中央値は $ 30 $ - $ (20) $ の中央値は $ 20 $ - $ (10,\ 30) $ の中央値は $ 30 $ - $ (30,\ 20) $ の中央値は $ 30 $ - $ (10,\ 30,\ 20) $ の中央値は $ 20 $ よって、$ m\ =\ (10,\ 30,\ 20,\ 30,\ 30,\ 20) $ となり、$ m $ の中央値は $ 30 $ です。