# AT_abc351_f [ABC351F] Double Sum

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc351/tasks/abc351_f

整数列 $ A\ =\ (A_1,\ A_2,\ \dots,\ A_N) $ が与えられます。  
 次の式を計算してください。

$ \displaystyle\ \sum_{i=1}^N\ \sum_{j=i+1}^N\ \max(A_j\ -\ A_i,\ 0) $

なお、制約下において答えが $ 2^{63} $ 未満となることは保証されています。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \dots $ $ A_N $

## 输出格式

式の値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
2 5 3
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
10
5 9 3 0 4 8 7 5 4 0
```

### 输出 #2

```
58
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 4\ \times\ 10^5 $
- $ 0\ \leq\ A_i\ \leq\ 10^8 $
- 入力される値は全て整数
 
### Sample Explanation 1

$ (i,\ j)\ =\ (1,\ 2) $ のとき $ \max(A_j\ -\ A_i,\ 0)\ =\ \max(3,\ 0)\ =\ 3 $ です。 $ (i,\ j)\ =\ (1,\ 3) $ のとき $ \max(A_j\ -\ A_i,\ 0)\ =\ \max(1,\ 0)\ =\ 1 $ です。 $ (i,\ j)\ =\ (2,\ 3) $ のとき $ \max(A_j\ -\ A_i,\ 0)\ =\ \max(-2,\ 0)\ =\ 0 $ です。 これらを足し合わせた $ 3\ +\ 1\ +\ 0\ =\ 4 $ が答えとなります。