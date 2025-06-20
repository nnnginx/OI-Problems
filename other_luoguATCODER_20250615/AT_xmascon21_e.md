# AT_xmascon21_e E and PI

## 题目描述

[problemUrl]: https://atcoder.jp/contests/xmascon21/tasks/xmascon21_e

$ e\ =\ 2.718\cdots $ を自然対数の底，$ \pi\ =\ 3.141\cdots $ を円周率とする．

正の整数 $ n $ に対し，実数 $ f(n) $ を以下のように定める．座標平面上の中心 $ (0,\ 0) $ 半径 $ 1 $ の円 $ C $ を考える．$ C $ 上の点 $ P_0,\ P_1,\ \ldots,\ P_{n-1} $ を，$ P_j $ の座標を $ (\cos(2\ \pi\ e\ j),\ \sin(2\ \pi\ e\ j)) $ として定める ($ j\ =\ 0,\ 1,\ \ldots,\ n\ -\ 1 $)．$ P_0,\ P_1,\ \ldots,\ P_{n-1} $ は相異なることが証明できるので，$ C $ はこれらの点によって $ n $ 個の弧に分かれる．それらの長さのうちの最大値を $ f(n) $ とする．

 ![](https://cdn.luogu.com.cn/upload/vjudge_pic/AT_xmascon21_e/20bb53dffb63452d845c76323b6f4adf5be61162.png)$ n\ =\ 10 $ のときの様子

 

$ f(n)\ >\ f(n\ +\ 1) $ を満たす正の整数 $ n $ は無限個存在することが証明できる．それらを昇順に $ n_1,\ n_2,\ \ldots $ とする．

正の整数 $ K $ が与えられる．$ f(n_K)\ =\ 2\ \pi\ (a\ +\ e\ b) $ を満たす整数 $ a,\ b $ が一意に存在することが証明できる．$ n_K,\ a,\ b $ をそれぞれ $ 998244353 $ で割った余り ($ 0 $ 以上 $ 998244353 $ 未満) を求めよ．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ K $

## 输出格式

$ n_K,\ a,\ b $ をそれぞれ $ 998244353 $ で割った余りを順に出力せよ．

## 输入输出样例 #1

### 输入 #1

```
1
```

### 输出 #1

```
1 1 0
```

## 输入输出样例 #2

### 输入 #2

```
2
```

### 输出 #2

```
2 998244351 1
```

## 输入输出样例 #3

### 输入 #3

```
5
```

### 输出 #3

```
10 998244345 3
```

## 说明/提示

### 制約

- $ 1\ \le\ K\ \le\ 10^{11} $．

### Sample Explanation 1

$ n_1\ =\ 1 $，$ f(1)\ =\ 2\ \pi $ である．

### Sample Explanation 2

$ n_2\ =\ 2 $，$ f(2)\ =\ 2\ \pi\ (-2\ +\ e) $ である．

### Sample Explanation 3

$ n_5\ =\ 10 $，$ f(10)\ =\ 2\ \pi\ (-8\ +\ 3\ e) $ である．