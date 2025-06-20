# AT_agc043_c [AGC043C] Giant Graph

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc043/tasks/agc043_c

$ N $ 頂点の、それぞれ $ M_1 $, $ M_2 $, $ M_3 $ 辺の単純な無向グラフ $ X $, $ Y $, $ Z $ が与えられます。 頂点をそれぞれ $ x_1,\ x_2,\ \dots,\ x_N $, $ y_1,\ y_2,\ \dots,\ y_N $, $ z_1,\ z_2,\ \dots,\ z_N $ とします。 $ X $, $ Y $, $ Z $ の辺はそれぞれ $ (x_{a_i},\ x_{b_i}) $, $ (y_{c_i},\ y_{d_i}) $, $ (z_{e_i},\ z_{f_i}) $ です。

$ X,\ Y,\ Z $ を元に $ N^3 $ 頂点の無向グラフ $ W $ を作ります。 $ X,\ Y,\ Z $ から $ 1 $ つずつ頂点を選ぶ方法は $ N^3 $ 通りありますが、これがそれぞれ $ W $ の頂点と一対一に対応します。$ x_i,\ y_j,\ z_k $ を選ぶことに対応する頂点を $ (x_i,\ y_j,\ z_k) $ で表すこととします。

$ W $ の辺を、以下の手順に沿って張ります。

- $ X $ の各辺 $ (x_u,\ x_v) $、及び全ての $ w,\ l $ について、$ (x_u,\ y_w,\ z_l) $, $ (x_v,\ y_w,\ z_l) $ 間に辺を張る
- $ Y $ の各辺 $ (y_u,\ y_v) $、及び全ての $ w,\ l $ について、$ (x_w,\ y_u,\ z_l) $, $ (x_w,\ y_v,\ z_l) $ 間に辺を張る
- $ Z $ の各辺 $ (z_u,\ z_v) $、及び全ての $ w,\ l $ について、$ (x_w,\ y_l,\ z_u) $, $ (x_w,\ y_l,\ z_v) $ 間に辺を張る

そして、$ W $ の頂点 $ (x_i,\ y_j,\ z_k) $ の重みを $ 1,000,000,000,000,000,000^{(i\ +j\ +\ k)}\ =\ 10^{18(i\ +\ j\ +\ k)} $ とします。$ W $ の[独立集合](https://ja.wikipedia.org/wiki/%E7%8B%AC%E7%AB%8B%E9%9B%86%E5%90%88)のうち、頂点の重みの総和の最大値を求めてください。そしてそれを $ 998,244,353 $ で割った余りを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M_1 $ $ a_1 $ $ b_1 $ $ a_2 $ $ b_2 $ $ \vdots $ $ a_{M_1} $ $ b_{M_1} $ $ M_2 $ $ c_1 $ $ d_1 $ $ c_2 $ $ d_2 $ $ \vdots $ $ c_{M_2} $ $ d_{M_2} $ $ M_3 $ $ e_1 $ $ f_1 $ $ e_2 $ $ f_2 $ $ \vdots $ $ e_{M_3} $ $ f_{M_3} $

## 输出格式

重みの総和の最大値を $ 998,244,353 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2
1
1 2
1
1 2
1
1 2
```

### 输出 #1

```
46494701
```

## 输入输出样例 #2

### 输入 #2

```
3
3
1 3
1 2
3 2
2
2 1
2 3
1
2 1
```

### 输出 #2

```
883188316
```

## 输入输出样例 #3

### 输入 #3

```
100000
1
1 2
1
99999 100000
1
1 100000
```

### 输出 #3

```
318525248
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 100,000 $
- $ 1\ \leq\ M_1,\ M_2,\ M_3\ \leq\ 100,000 $
- $ 1\ \leq\ a_i,\ b_i,\ c_i,\ d_i,\ e_i,\ f_i\ \leq\ N $
- $ X $, $ Y $, $ Z $ は単純、つまり自己ループや多重辺は存在しない

### Sample Explanation 1

$ (x_2,\ y_1,\ z_1) $, $ (x_1,\ y_2,\ z_1) $, $ (x_1,\ y_1,\ z_2) $, $ (x_2,\ y_2,\ z_2) $ を選ぶ場合が最適です。 答えは $ 3\ \times\ 10^{72}\ +\ 10^{108} $ を $ 998,244,353 $ で割ったあまりの $ 46,494,701 $ です。