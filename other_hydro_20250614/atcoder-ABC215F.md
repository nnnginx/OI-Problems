## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc215/tasks/abc215_f

$ 2 $ 次元平面上の $ N $ 個の相異なる点が与えられます。点 $ i\,\ (1\ \leq\ i\ \leq\ N) $ の座標は $ (x_i,y_i) $ です。

$ 2 $ つの点 $ i,j\,\ (1\ \leq\ i,j\ \leq\ N) $ の距離を $ \mathrm{min}\ (|x_i-x_j|,|y_i-y_j|) $ 、すなわち $ x $ 座標の差と $ y $ 座標の差の小さい方と定義します。

異なる $ 2 $ つの点の距離の最大値を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ x_1 $ $ y_1 $ $ x_2 $ $ y_2 $ $ \vdots $ $ x_N $ $ y_N $

## 输出格式
異なる $ 2 $ つの点の距離の最大値を出力せよ。

## 题目大意
给定 $n$ 个二维平面上的点 $(x_i, y_i)$，求 $\max\limits_{1\le i<j\le n}^n \Big(\min(\left| x_i - x_j\right|, \left|y_i - y_j\right|)\Big)$。

translated by @[liangbowen](https://www.luogu.com.cn/user/367488)。

```input1
3
0 3
3 1
4 10
```

```output1
4
```

```input2
4
0 1
0 4
0 10
0 6
```

```output2
0
```

```input3
8
897 729
802 969
765 184
992 887
1 104
521 641
220 909
380 378
```

```output3
801
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 200000 $
- $ 0\ \leq\ x_i,y_i\ \leq\ 10^9 $
- $ (x_i,y_i) $ $ \neq $ $ (x_j,y_j) $ $ (i\ \neq\ j) $
- 入力は全て整数である。

### Sample Explanation 1

点 $ 1 $ と点 $ 2 $ の距離は $ 2 $ 、点 $ 1 $ と点 $ 3 $ の距離は $ 4 $ 、点 $ 2 $ と点 $ 3 $ の距離は $ 1 $ です。よって $ 4 $ を出力してください。

