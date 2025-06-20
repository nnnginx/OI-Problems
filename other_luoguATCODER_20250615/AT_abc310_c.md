# AT_abc310_c [ABC310C] Reversible

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc310/tasks/abc310_c

ボールがいくつか刺さった棒が $ N $ 本あり、各ボールには英小文字が $ 1 $ 個書かれています。

$ i\ =\ 1,\ 2,\ \ldots,\ N $ について、$ i $ 番目の棒に刺さった各ボールの英小文字は、文字列 $ S_i $ によって表されます。 具体的には、$ i $ 番目の棒には文字列 $ S_i $ の長さ $ |S_i| $ に等しい個数のボールが刺さっており、 刺さっているボールの英小文字を、棒のある端から順に並べたものは文字列 $ S_i $ と等しいです。

$ 2 $ つの棒は、一方の棒に刺さっているボールの英小文字をどちらかの端から並べた列と、もう一方の棒に刺さっているボールの英小文字をどちらかの端から並べた列が一致するとき、同じ棒とみなされます。 より形式的には、$ 1 $ 以上 $ N $ 以下の整数 $ i,\ j $ について、$ i $ 本目の棒と $ j $ 本目の棒は、$ S_i $ が $ S_j $ と一致するか、$ S_i $ が $ S_j $ を前後反転したものと一致するとき、かつそのときに限り、同じとみなされます。

$ N $ 本の棒の中に、何種類の異なる棒があるかを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
6
a
abc
de
cba
de
abc
```

### 输出 #1

```
3
```

## 说明/提示

### 制約

- $ N $ は整数
- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ S_i $ は英小文字のみからなる文字列
- $ |S_i|\ \geq\ 1 $
- $ \sum_{i\ =\ 1}^N\ |S_i|\ \leq\ 2\ \times\ 10^5 $
 
### Sample Explanation 1

\- $ S_2 $ = `abc` が $ S_4 $ = `cba` を前後反転したものと一致するため、$ 2 $ 番目の棒と $ 4 $ 番目の棒は同じとみなされます。 - $ S_2 $ = `abc` が $ S_6 $ = `abc` と一致するため、$ 2 $ 番目の棒と $ 6 $ 番目の棒は同じとみなされます。 - $ S_3 $ = `de` が $ S_5 $ = `de` と一致するため、$ 3 $ 番目の棒と $ 5 $ 番目の棒は同じとみなされます。 よって、$ 6 $ 本の棒の中に、$ 1 $ 本目の棒、$ 2 $ 本目の棒（ $ 4,\ 6 $ 本目の棒と同じ）、$ 3 $ 本目の棒（ $ 5 $ 本目の棒と同じ）の $ 3 $ 種類の異なる棒があります。