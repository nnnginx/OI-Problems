# AT_arc107_e [ARC107E] Mex Mat

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc107/tasks/arc107_e

$ N\ \times\ N $ の行列を考えます。この行列の $ i $ 行目、$ j $ 列目の値を $ a_{i,\ j} $ とします。$ i\ =\ 1 $ か $ j\ =\ 1 $ を満たす $ a_{i,\ j} $ については $ 0 $, $ 1 $, $ 2 $ のいずれかの値が入力で与えられます。残りの値は以下の規則に従い定めます。

- $ a_{i,j}\ =\ \mathrm{mex}(a_{i-1,j},\ a_{i,j-1})\ (2\ \leq\ i,\ j\ \leq\ N) $。ただし $ \mathrm{mex}(x,\ y) $ は次の表に従う。
 
$ \mathrm{mex}(x,\ y) $ $ y=0 $ $ y=1 $ $ y=2 $ $ x=0 $ $ 1 $ $ 2 $ $ 1 $ $ x=1 $ $ 2 $ $ 0 $ $ 0 $ $ x=2 $ $ 1 $ $ 0 $ $ 0 $行列の要素のうち、値が $ 0,\ 1,\ 2 $ であるものはそれぞれ何個でしょうか？

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ a_{1,\ 1} $ $ a_{1,\ 1} $ $ ... $ $ a_{1,\ N} $ $ a_{2,\ 1} $ $ : $ $ a_{N,\ 1} $

## 输出格式

$ 0 $ の個数、$ 1 $ の個数、$ 2 $ の個数を空白区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
1 2 0 2
0
0
0
```

### 输出 #1

```
7 4 5
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 500{,}000 $
- 入力される $ a_{i,\ j} $ の値はすべて $ 0,\ 1,\ 2 $ のいずれか

### Sample Explanation 1

行列は以下のようになります。 ``` 1 2 0 2 0 1 2 0 0 2 0 1 0 1 2 0 ```