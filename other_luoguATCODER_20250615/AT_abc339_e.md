# AT_abc339_e [ABC339E] Smooth Subsequence

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc339/tasks/abc339_e

長さ $ N $ の数列 $ A\ =\ (A_1,\ A_2,\ \ldots,\ A_N) $ が与えられます。

$ A $ の部分列であって、隣接する $ 2 $ 項の差の絶対値が $ D $ 以下であるようなものの長さの最大値を求めてください。

ただし、数列 $ A $ の部分列とは、$ A $ の要素を $ 0 $ 個以上選んで削除し、残った要素を元の順序を保って並べた数列のことを指します。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ D $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 2
3 5 1 2
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
5 10
10 20 100 110 120
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
11 7
21 10 3 19 28 12 11 3 3 15 16
```

### 输出 #3

```
6
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 5\ \times\ 10^5 $
- $ 0\ \leq\ D\ \leq\ 5\ \times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 5\ \times\ 10^5 $
- 入力される数値はすべて整数
 
### Sample Explanation 1

$ A $ の部分列 $ (3,\ 1,\ 2) $ は隣接する $ 2 $ 項の差の絶対値が $ 2 $ 以下です。