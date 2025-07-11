# AT_agc037_f [AGC037F] Counting of Subarrays

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc037/tasks/agc037_f

正整数列 $ S $ 及び正整数 $ k,l $ が以下のいずれかの条件をみたすとき、 $ S $ が  **レベル**  $ (k,l) $ に属すると定義することにします。

- $ S $ の要素数が $ 1 $ であり、その要素の値が $ k $ である。
- あるレベル$ (k-1,l) $ に属する数列 $ T_1,T_2,...,T_m $ ($ m\ ≧\ l $) が存在して、 $ T_1,T_2,...,T_m $ をこの順に連結して得られる数列と $ S $ が一致する。

ただし、$ k=1 $ のとき二番目の条件は意味を持たない、つまりレベル$ (1,l) $の正整数列は一つ目の条件をみたすもののみであることに注意して下さい。

正整数列 $ A_1,A_2,...,A_N $ と正整数 $ L $ が与えられます。 以下の条件をみたす部分列 $ A_i,A_{i+1},...,A_j $ ($ 1\ ≦\ i\ ≦\ j\ ≦\ N $) の個数を求めてください。

- ある正整数 $ K $ が存在して、数列 $ A_i,A_{i+1},...,A_j $ がレベル$ (K,L) $に属する。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ L $ $ A_1 $ $ A_2 $ $ ... $ $ A_N $

## 输出格式

条件をみたす部分列の個数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
9 3
2 1 1 1 1 1 1 2 3
```

### 输出 #1

```
22
```

## 输入输出样例 #2

### 输入 #2

```
9 2
2 1 1 1 1 1 1 2 3
```

### 输出 #2

```
41
```

## 输入输出样例 #3

### 输入 #3

```
15 3
4 3 2 1 1 1 2 3 2 2 1 1 1 2 2
```

### 输出 #3

```
31
```

## 说明/提示

### 制約

- $ 1\ ≦\ N\ ≦\ 2\ \times\ 10^5 $
- $ 2\ ≦\ L\ ≦\ N $
- $ 1\ ≦\ A_i\ ≦\ 10^9 $

### Sample Explanation 1

例えば $ (1,1,1) $ と $ (2) $ という数列はともにレベル $ (2,3) $ に属するので、$ (2,1,1,1,1,1,1) $ という数列はレベル $ (3,3) $ に属します。