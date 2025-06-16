# AT_abc177_c [ABC177C] Sum of product of pairs

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc177/tasks/abc177_c

$ N $ 個の整数 $ A_1,\ldots,A_N $ が与えられます。

$ 1\leq\ i\ <\ j\ \leq\ N $ を満たす全ての組 $ (i,j) $ についての $ A_i\ \times\ A_j $ の和を $ \bmod\ (10^9+7) $ で求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ \ldots $ $ A_N $

## 输出格式

$ \sum_{i=1}^{N-1}\sum_{j=i+1}^{N}\ A_i\ A_j $ を $ \bmod\ (10^9+7) $ で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
1 2 3
```

### 输出 #1

```
11
```

## 输入输出样例 #2

### 输入 #2

```
4
141421356 17320508 22360679 244949
```

### 输出 #2

```
437235829
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 0\ \leq\ A_i\ \leq\ 10^9 $
- 入力は全て整数

### Sample Explanation 1

$ 1\ \times\ 2\ +\ 1\ \times\ 3\ +\ 2\ \times\ 3\ =\ 11 $ です。