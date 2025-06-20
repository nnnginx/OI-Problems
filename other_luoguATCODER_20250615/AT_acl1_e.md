# AT_acl1_e Shuffle Window

## 题目描述

[problemUrl]: https://atcoder.jp/contests/acl1/tasks/acl1_e

$ (1,\ 2,\ ...,\ N) $ の順列 $ p_1,\ p_2,\ \dots,\ p_N $ と整数 $ K $ が与えられます。 maroonくんは $ i\ =\ 1,\ 2,\ \dots,\ N\ -\ K\ +\ 1 $ について、次の操作を順番に行います。

- $ p_i,\ p_{i\ +\ 1},\ \dots,\ p_{i\ +\ K\ -\ 1} $ を一様ランダムにシャッフルする。

すべての操作の後の数列の転倒数の期待値を求め、$ \bmod\ 998244353 $ で出力してください。

より正確には、期待値が有理数、つまりある既約分数 $ \frac{P}{Q} $ で表せること、更に $ R\ \times\ Q\ \equiv\ P\ \pmod{998244353},\ 0\ \leq\ R\ <\ 998244353 $ を満たす整数 $ R $ が一意に定まることがこの問題の制約より証明できます。よって、この $ R $ を出力してください。

また、数列 $ a_1,\ a_2,\ \dots,\ a_N $ の転倒数とは、$ i\ <\ j,\ a_i\ >\ a_j $ を満たす順序対 $ (i,\ j) $ の個数とします。

## 输入格式

> $ N $ $ K $ $ p_1 $ $ p_2 $ ... $ p_N $

## 输出格式

期待値を $ \bmod\ 998244353 $ で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 2
1 2 3
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
10 3
1 8 4 9 2 3 7 10 5 6
```

### 输出 #2

```
164091855
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 200,000 $
- $ 2\ \leq\ K\ \leq\ N $
- $ (p_1,\ p_2,\ \dots,\ p_N) $ は $ (1,\ 2,\ \dots,\ N) $ の並び替え
- 入力される数は全て整数である．

### Sample Explanation 1

$ (1,\ 2,\ 3) $, $ (2,\ 1,\ 3) $, $ (1,\ 3,\ 2) $, $ (2,\ 3,\ 1) $ が、それぞれ $ \frac{1}{4} $ の確率で最終的な数列になります。 これらの転倒数は $ 0,\ 1,\ 1,\ 2 $ なので、期待値は $ 1 $ です。