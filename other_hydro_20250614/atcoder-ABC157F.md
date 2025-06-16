## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc157/tasks/abc157_f

高橋君は二次元平面である網の上で $ N $ 枚の肉を焼こうとしています。 $ i $ 枚目の肉の位置は $ \left(x_i,\ y_i\right) $であり、火の通りにくさは $ c_i $ です。

高橋君は熱源を $ 1 $ つ持っています。熱源を位置 $ \left(X,\ Y\right) $ ($ X,\ Y $は実数)に置くと、 $ i $枚目の肉は、 焼けるまでに $ c_i\ \times\ \sqrt{\left(X\ -\ x_i\right)^2\ +\ \left(Y-y_i\right)^2} $ 秒掛かります。

高橋君は肉を $ K $ 枚食べたいと考えています。 $ K $ 枚以上の肉が焼けるまでに掛かる時間を最小化するように高橋君が熱源を配置したとき、その所要時間を求めてください。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ x_1 $ $ y_1 $ $ c_1 $ $ \vdots $ $ x_N $ $ y_N $ $ c_N $

## 输出格式
答えを出力せよ。

なお、想定解答との絶対誤差または相対誤差が $ 10^{-6} $ 以下であれば正解として扱われる。

## 题目大意
给定平面直角坐标系内的 $N$ 个点 ，每个点的坐标为 $(x_i\ ,\ y_i)$，且有一个系数 $c_i$ 。

请选择一个点 $(\text{X}\ ,\ \text{Y})$ ，最小化 $c_i\times\sqrt{{(\text{X}-x_i)}^2+{(\text{Y}-y_i)}^2}$ 的 $K$ 小值。

输出该 $K$ 小值 ，误差不超过 $10^{-6}$ 即视为正确 。

数据范围：$1 \leqslant K \leqslant N \leqslant 60\ ,-1000 \leqslant x_i\ ,\ y_i \leqslant 1000\ ,1 \leqslant c_i \leqslant 100$ ，无重复点。

```input1
4 3
-1 0 3
0 0 3
1 0 2
1 1 40
```

```output1
2.4
```

```input2
10 5
-879 981 26
890 -406 81
512 859 97
362 -955 25
128 553 17
-885 763 2
449 310 57
-656 -204 11
-270 76 40
184 170 16
```

```output2
7411.2252
```

## 提示
### 制約

- 入力は全て整数
- $ 1\ \leq\ N\ \leq\ 60 $
- $ 1\ \leq\ K\ \leq\ N $
- $ -1000\ \leq\ x_i\ ,\ y_i\ \leq\ 1000 $
- $ \left(x_i,\ y_i\right)\ \neq\ \left(x_j,\ y_j\right)\ \left(i\ \neq\ j\ \right) $
- $ 1\ \leq\ c_i\ \leq\ 100 $

### Sample Explanation 1

熱源を $ \left(-0.2,\ 0\right) $に置くと、 $ 2.4 $ 秒後までに $ 1,\ 2,\ 3 $ 枚目の肉が焼けます。これが最適な熱源の置き方です。

