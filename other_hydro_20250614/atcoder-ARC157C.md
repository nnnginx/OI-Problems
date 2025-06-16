## 题目描述
[problemUrl]: https://atcoder.jp/contests/arc157/tasks/arc157_c

$ H $ 行 $ W $ 列のマス目の各マスに `X`, `Y` のいずれかの文字が書かれています． 上から $ i $ 行目，左から $ j $ 列目のマスを $ (i,\ j) $ で表します． マス目に書かれている文字は $ H $ 個の文字列 $ S_1,\ S_2,\ \dots,\ S_H $ によって与えられ，$ S_i $ の $ j $ 文字目がマス $ (i,\ j) $ に書かれた文字を表します．

下または右に隣接するマスへの移動を繰り返してマス $ (1,\ 1) $ からマス $ (H,\ W) $ に至る経路 $ P $ に対して，

- 「 $ P $ で通るマスに書かれた文字を順に並べて得られる長さ $ (H\ +\ W\ -\ 1) $ の文字列」を $ \mathrm{str}(P) $ とし，
- 「 $ \mathrm{str}(P) $ 中で `Y` 同士が隣り合う箇所の**個数の $ 2 $ 乗**」を $ P $ の**スコア**と定義します．
 
そのような経路 $ P $ としてあり得るものは $ \displaystyle\binom{H\ +\ W\ -\ 2}{H\ -\ 1} $ 通りありますが，その全てに対するスコアの総和を $ 998244353 $ で割った余りを求めてください．

  $ \binom{N}{K} $ の意味 $ \displaystyle\binom{N}{K} $ は，$ N $ 個の相異なる要素から $ K $ 個を選ぶ場合の数を表す二項係数です．

## 输入格式
入力は以下の形式で標準入力から与えられる．

> $ H $ $ W $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_H $

## 输出格式
あり得る経路全てに対するスコアの総和を $ 998244353 $ で割った余りを出力せよ．

## 题目大意
给定 $H \times W$ 的矩阵，每个位置上有一个字符，是 `X` 或 `Y`。

定义一条路径的权值为，将其经过的字符按顺序拼接成一个字符串，`YY` 在这个字符串的出现次数。

要求每次只能向右或向下走，求，所有的 $\binom{H + W - 2}{H - 1}$ 条左上到右下的路径，它们权值平方的和。

```input1
2 2
YY
XY
```

```output1
4
```

```input2
2 2
XY
YY
```

```output2
2
```

```input3
10 20
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
YYYYYYYYYYYYYYYYYYYY
```

```output3
423787835
```

## 提示
### 制約

- $ 1\ \leq\ H\ \leq\ 2000 $
- $ 1\ \leq\ W\ \leq\ 2000 $
- $ S_i\ (1\ \leq\ i\ \leq\ H) $ は `X`, `Y` からなる長さ $ W $ の文字列である．
 
### Sample Explanation 1

経路 $ P $ としてあり得るものは $ (1,\ 1)\ \to\ (1,\ 2)\ \to\ (2,\ 2) $ と $ (1,\ 1)\ \to\ (2,\ 1)\ \to\ (2,\ 2) $ の $ 2 $ 通りです． - $ (1,\ 1)\ \to\ (1,\ 2)\ \to\ (2,\ 2) $ の場合，$ \mathrm{str}(P)\ =\ {} $`YYY` であり，$ 1,\ 2 $ 文字目と $ 2,\ 3 $ 文字目の $ 2 $ 箇所で `Y` 同士が隣り合っているので，スコアは $ 2^2\ =\ 4 $ です． - $ (1,\ 1)\ \to\ (2,\ 1)\ \to\ (2,\ 2) $ の場合，$ \mathrm{str}(P)\ =\ {} $`YXY` であり，`Y` 同士が隣り合う箇所は無いので，スコアは $ 0^2\ =\ 0 $ です． したがって，求める総和は $ 4\ +\ 0\ =\ 4 $ となります．

### Sample Explanation 2

$ 2 $ 通りのいずれの経路の場合も $ \mathrm{str}(P)\ =\ {} $`XYY` であり，スコアは $ 1^2\ =\ 1 $ です．

### Sample Explanation 3

スコアの総和を $ 998244353 $ で割った余りを出力してください．

