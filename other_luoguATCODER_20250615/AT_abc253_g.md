# AT_abc253_g [ABC253G] Swap Many Times

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc253/tasks/abc253_g

$ 2 $ 以上の整数 $ N $ に対し、$ 1\ \leq\ x\ \lt\ y\ \leq\ N $ を満たす整数の組 $ (x,\ y) $ は $ \frac{N(N\ -\ 1)}{2} $ 個あります。

これらを辞書順で小さい順に並べたもののうち $ L $ 番目、$ L+1 $ 番目、$ \ldots $、$ R $ 番目のものをそれぞれ $ (x_1,\ y_1),\ \dots,\ (x_{R\ -\ L\ +\ 1},\ y_{R\ -\ L\ +\ 1}) $ とおきます。数列 $ A\ =\ (1,\ \dots,\ N) $ に対し、$ i\ =\ 1,\ \dots,\ R-L+1 $ の順に以下の操作を行います。

- $ A_{x_i} $ と $ A_{y_i} $ を入れ替える

操作後の $ A $ を求めてください。

なお、$ (a,\ b) $ が $ (c,\ d) $ よりも辞書順で小さいとは、以下のいずれかが成り立つことをいいます。

- $ a\ \lt\ c $
- $ a\ =\ c $ かつ $ b\ \lt\ d $

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ L $ $ R $

## 输出格式

操作後の $ A $ の各項を空白区切りで一行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 3 6
```

### 输出 #1

```
5 1 2 3 4
```

## 输入输出样例 #2

### 输入 #2

```
10 12 36
```

### 输出 #2

```
1 10 9 8 7 4 3 2 5 6
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ L\ \leq\ R\ \leq\ \frac{N(N-1)}{2} $
- 入力は全て整数

### Sample Explanation 1

$ 1\ \leq\ x\ \lt\ y\ \leq\ N $ を満たす整数の組を辞書順で小さい順に並べたもののうち $ 3,\ 4,\ 5,\ 6 $ 番目のものはそれぞれ $ (1,\ 4),\ (1,\ 5),\ (2,\ 3),\ (2,\ 4) $ です。 これらについて順に操作を行うと、$ A $ は次のように変化します。 $ (1,\ 2,\ 3,\ 4,\ 5)\ \rightarrow\ (4,\ 2,\ 3,\ 1,\ 5)\ \rightarrow\ (5,\ 2,\ 3,\ 1,\ 4)\ \rightarrow\ (5,\ 3,\ 2,\ 1,\ 4)\ \rightarrow\ (5,\ 1,\ 2,\ 3,\ 4) $