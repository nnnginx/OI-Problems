# AT_abc164_f [ABC164F] I hate Matrix Construction

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc164/tasks/abc164_f

整数 $ N $ 及び長さ $ N $ の配列 $ S $, $ T $, $ U $, $ V $ が与えられます。 以下の条件を満たすような $ N×N $ の行列 $ a $ をどれか $ 1 $ つ構築してください。

- $ a_{i,j} $ は整数である。
- $ 0\ \leq\ a_{i,j}\ \lt\ 2^{64} $
- $ S_{i}\ =\ 0 $ のとき $ i $ 行目の要素のビットごとの論理積は $ U_{i} $ である。
- $ S_{i}\ =\ 1 $ のとき $ i $ 行目の要素のビットごとの論理和は $ U_{i} $ である。
- $ T_{i}\ =\ 0 $ のとき $ i $ 列目の要素のビットごとの論理積は $ V_{i} $ である。
- $ T_{i}\ =\ 1 $ のとき $ i $ 列目の要素のビットごとの論理和は $ V_{i} $ である。

ただし、条件を満たす行列が存在しない場合もあるかもしれません。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_{1} $ $ S_{2} $ $ ... $ $ S_{N} $ $ T_{1} $ $ T_{2} $ $ ... $ $ T_{N} $ $ U_{1} $ $ U_{2} $ $ ... $ $ U_{N} $ $ V_{1} $ $ V_{2} $ $ ... $ $ V_{N} $

## 输出格式

条件を満たす行列が存在する場合は、そのような行列 $ 1 $ つを以下の形式で出力せよ。

> $ a_{1,1} $ $ ... $ $ a_{1,N} $ $ : $ $ a_{N,1} $ $ ... $ $ a_{N,N} $

条件を満たす行列なら何を出力してもいいことに注意せよ。

条件を満たす行列が存在しない場合は $ -1 $ を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2
0 1
1 0
1 1
1 0
```

### 输出 #1

```
1 1
1 0
```

## 输入输出样例 #2

### 输入 #2

```
2
1 1
1 0
15 15
15 11
```

### 输出 #2

```
15 11
15 11
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 1\ \leq\ N\ \leq\ 500 $
- $ 0\ \leq\ S_{i}\ \leq\ 1 $
- $ 0\ \leq\ T_{i}\ \leq\ 1 $
- $ 0\ \leq\ U_{i}\ \lt\ 2^{64} $
- $ 0\ \leq\ V_{i}\ \lt\ 2^{64} $

### Sample Explanation 1

入力例 $ 1 $ では - $ 1 $ 行目の要素のビットごとの論理積が $ 1 $ - $ 2 $ 行目の要素のビットごとの論理和が $ 1 $ - $ 1 $ 列目の要素のビットごとの論理和が $ 1 $ - $ 2 $ 列目の要素のビットごとの論理積が $ 0 $ の条件を満たす行列を見つける必要があります。