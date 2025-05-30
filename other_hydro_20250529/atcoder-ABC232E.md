## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc232/tasks/abc232_e

縦 $ H $ 行、横 $ W $ 行の $ H\ \times\ W $ マスからなるグリッドがあります。上から $ i $ 行目、左から $ j $ 列目のマスを $ (i,\ j) $ と表します。

はじめ、マス $ (x_1,\ y_1) $ にルークが置かれており、高橋君は以下の操作を $ K $ 回行います。

- 現在ルークが置かれているマスと行または列が同じマスにルークを移動させる。ただし、現在ルークが置かれているマスとは異なるマスに移動させる必要がある。

$ K $ 回の操作の後、ルークがマス $ (x_2,\ y_2) $ に置かれているようにする方法は何通りありますか？答えは非常に大きくなることがあるので、$ 998244353 $ で割った余りを求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ H $ $ W $ $ K $ $ x_1 $ $ y_1 $ $ x_2 $ $ y_2 $

## 输出格式
$ K $ 回の操作の後、ルークがマス $ (x_2,\ y_2) $ に置かれているようにする方法の総数を $ 998244353 $ で割った余りを出力せよ。

## 题目大意
有一个 $H\times W$ 的国际象棋棋盘，求一个**车**从 $(x_1,y_1)$ 走到 $(x_2,y_2)$ 正好用 $K$ 步的方案数。

Translated by @[$\tt{\_YXJS\_}$](/user/516346).

```input1
2 2 2
1 2 2 1
```

```output1
2
```

```input2
1000000000 1000000000 1000000
1000000000 1000000000 1000000000 1000000000
```

```output2
24922282
```

```input3
3 3 3
1 3 3 3
```

```output3
9
```

## 提示
### 制約

- $ 2\ \leq\ H,\ W\ \leq\ 10^9 $
- $ 1\ \leq\ K\ \leq\ 10^6 $
- $ 1\ \leq\ x_1,\ x_2\ \leq\ H $
- $ 1\ \leq\ y_1,\ y_2\ \leq\ W $

### Sample Explanation 1

以下の $ 2 $ 通りです。 - $ 1 $ 回目の操作でルークをマス $ (1,\ 2) $ からマス $ (1,\ 1) $ へ動かし、$ 2 $ 回目の操作でルークをマス $ (1,\ 1) $ からマス $ (2,\ 1) $ に動かす。 - $ 1 $ 回目の操作でルークをマス $ (1,\ 2) $ からマス $ (2,\ 2) $ へ動かし、$ 2 $ 回目の操作でルークをマス $ (2,\ 2) $ からマス $ (2,\ 1) $ に動かす。

### Sample Explanation 2

$ 998244353 $ で割った余りを求めなければならないことに注意して下さい。

