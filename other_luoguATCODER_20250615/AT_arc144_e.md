# AT_arc144_e [ARC144E] GCD of Path Weights

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc144/tasks/arc144_e

$ N $ 頂点 $ M $ 辺からなる有向グラフ $ G $ が与えられます．頂点には $ 1,\ 2,\ \ldots,\ N $ の番号がついています．$ i $ 番目の辺は $ a_i $ から $ b_i $ に向かう有向辺で，$ a_i\ <\ b_i $ が成り立っています．

正整数列 $ W\ =\ (W_1,\ W_2,\ \ldots,\ W_N) $ の**美しさ**を，次が成り立つような正整数 $ x $ の最大値として定義します．

- $ G $ における頂点 $ 1 $ から頂点 $ N $ への任意のパス $ (v_1,\ \ldots,\ v_k) $ ($ v_1\ =\ 1,\ v_k\ =\ N $) に対し，$ \sum_{i=1}^k\ W_{v_i} $ は $ x $ の倍数である．

整数列 $ A\ =\ (A_1,\ A_2,\ \ldots,\ A_N) $ が与えられます．正整数列 $ W\ =\ (W_1,\ \ldots,\ W_N) $ を，$ A_i\ \neq\ -1\ \implies\ W_i\ =\ A_i $ を満たすように定めるとき，その美しさとしてありうる最大値を求めてください．ただし，最大値が存在しない場合には `-1` を出力してください．

## 输入格式

入力は以下の形式で標準入力から与えられます．

> $ N $ $ M $ $ a_1 $ $ b_1 $ $ \vdots $ $ a_M $ $ b_M $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

正整数列 $ W $ の美しさとしてありうる最大値を出力してください．ただし，最大値が存在しない場合には `-1` を出力してください．

## 输入输出样例 #1

### 输入 #1

```
4 4
1 2
1 3
2 4
3 4
-1 3 7 -1
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
4 5
1 2
1 3
2 4
3 4
1 4
-1 3 7 -1
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
4 4
1 2
1 3
2 4
3 4
3 -1 -1 7
```

### 输出 #3

```
-1
```

## 输入输出样例 #4

### 输入 #4

```
5 5
1 3
3 5
2 3
3 4
1 4
2 -1 3 -1 4
```

### 输出 #4

```
9
```

## 说明/提示

### 制約

- $ 2\leq\ N\leq\ 3\times\ 10^5 $
- $ 1\leq\ M\leq\ 3\times\ 10^5 $
- $ 1\leq\ a_i\ <\ b_i\ \leq\ N $
- $ i\neq\ j $ ならば $ (a_i,b_i)\neq\ (a_j,b_j) $
- 与えられるグラフ $ G $ において，頂点 $ 1 $ から頂点 $ N $ へのパスが存在する．
- $ A_i\ =\ -1 $ または $ 1\leq\ A_i\leq\ 10^{12} $

### Sample Explanation 1

頂点 $ 1 $ から頂点 $ N $ へのパスは，$ (1,2,4) $, $ (1,3,4) $ の $ 2 $ 個です． 例えば $ W\ =\ (5,\ 3,\ 7,\ 8) $ の美しさは $ 4 $ となります．実際，$ W_1\ +\ W_2\ +\ W_4\ =\ 16 $, $ W_1\ +\ W_3\ +\ W_4\ =\ 20 $ はともに $ 4 $ の倍数です．

### Sample Explanation 2

頂点 $ 1 $ から頂点 $ N $ へのパスは，$ (1,2,4) $, $ (1,3,4) $, $ (1,4) $ の $ 3 $ 個です． 例えば $ W\ =\ (5,\ 3,\ 7,\ 8) $ の美しさは $ 1 $ となります．

### Sample Explanation 3

例えば $ W\ =\ (3,\ 10^{100},\ 10^{100},\ 7) $ の美しさは $ 10^{100}+10 $ となります．$ W $ の美しさをいくらでも大きくできるため，その最大値は存在しません．