# AT_agc027_d [AGC027D] Modulo Matrix

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc027/tasks/agc027_d

整数 $ N $ が与えられます。

以下の条件を満たすような $ N\ \times\ N $ 行列 $ a $ をどれか $ 1 $ つ構成してください。この問題の制約下で、必ず解が存在することが証明できます。

- $ 1\ \leq\ a_{i,j}\ \leq\ 10^{15} $
- $ a_{i,j} $ は相異なる整数である
- ある正の整数 $ m $ が存在して、上下左右に隣接する $ 2 $ つの数 $ x,y $ をどこから取り出しても、$ {\rm\ max}(x,y) $ を $ {\rm\ min}(x,y) $ で割ったあまりは $ m $ となる

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式

答えを以下の形式で出力せよ。

> $ a_{1,1} $ $ ... $ $ a_{1,N} $ $ : $ $ a_{N,1} $ $ ... $ $ a_{N,N} $

## 输入输出样例 #1

### 输入 #1

```
2
```

### 输出 #1

```
4 7
23 10
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 500 $

### Sample Explanation 1

\- どの隣接した $ 2 $ つの数についても、大きい方の数を小さい数で割ったあまりが $ 3 $ となっています