# AT_abc201_e [ABC201E] Xor Distances

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc201/tasks/abc201_e

$ N $ 頂点の重み付き木があります。$ i $ 本目の辺は頂点 $ u_i $ と頂点 $ v_i $ を双方向に結んでいて、その重みは $ w_i $ です。

頂点の組 $ (x,y) $ について、$ \text{dist}(x,y) $ を以下のように定めます。

- $ x $ から $ y $ への最短パスに含まれる辺全ての重みの **XOR**

$ 1\ \leq\ i\ \lt\ j\ \leq\ N $ を満たす全ての組 $ (i,j) $ について $ \text{dist}(i,j) $ を求め、その総和を $ (10^9+7) $ で割った余りを出力してください。

 $ \text{\ XOR\ } $ とは 整数 $ a,\ b $ のビットごとの排他的論理和 $ a\ \text{\ XOR\ }\ b $ は、以下のように定義されます。

- $ a\ \text{\ XOR\ }\ b $ を二進表記した際の $ 2^k $ ($ k\ \geq\ 0 $) の位の数は、$ a,\ b $ を二進表記した際の $ 2^k $ の位の数のうち一方のみが $ 1 $ であれば $ 1 $、そうでなければ $ 0 $ である。
 
 例えば、$ 3\ \text{\ XOR\ }\ 5\ =\ 6 $ となります (二進表記すると: $ 011\ \text{\ XOR\ }\ 101\ =\ 110 $)。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ u_1 $ $ v_1 $ $ w_1 $ $ u_2 $ $ v_2 $ $ w_2 $ $ \vdots $ $ u_{N-1} $ $ v_{N-1} $ $ w_{N-1} $

## 输出格式

$ \text{dist}(i,j) $ の総和を $ (10^9+7) $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
1 2 1
1 3 3
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
5
3 5 2
2 3 2
1 5 1
4 5 13
```

### 输出 #2

```
62
```

## 输入输出样例 #3

### 输入 #3

```
10
5 7 459221860242673109
6 8 248001948488076933
3 5 371922579800289138
2 5 773108338386747788
6 10 181747352791505823
1 3 803225386673329326
7 8 139939802736535485
9 10 657980865814127926
2 4 146378247587539124
```

### 输出 #3

```
241240228
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ u_i\ \lt\ v_i\ \leq\ N $
- $ 0\ \leq\ w_i\ \lt\ 2^{60} $
- 与えられるグラフは木
- 入力は全て整数

### Sample Explanation 1

$ \text{dist}(1,2)=1, $ $ \text{dist}(1,3)=3, $ $ \text{dist}(2,3)=2 $ であり、これらの総和は $ 6 $ です。

### Sample Explanation 3

$ (10^9+7) $ で割った余りを出力してください。