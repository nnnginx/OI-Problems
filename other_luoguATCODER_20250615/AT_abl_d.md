# AT_abl_d Flat Subsequence

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abl/tasks/abl_d

数列 $ A_1,\ A_2,\ ...,\ A_N $ と整数 $ K $ が与えられます。

以下の条件を満たす数列 $ B $ の長さとして考えられる最大値を出力してください。

- $ B $ は $ A $ の (連続とは限らない) 部分列である。
- どの $ B $ の隣り合う要素の差の絶対値も $ K $ 以下である。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ : $ $ A_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
10 3
1
5
4
3
8
6
9
7
2
4
```

### 输出 #1

```
7
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 300,000 $
- $ 0\ \leq\ A_i\ \leq\ 300,000 $
- $ 0\ \leq\ K\ \leq\ 300,000 $
- 入力は全て整数である。

### Sample Explanation 1

たとえば、 $ B\ =\ (1,\ 4,\ 3,\ 6,\ 9,\ 7,\ 4) $ は条件を満たします。 - これは $ A\ =\ (1,\ 5,\ 4,\ 3,\ 8,\ 6,\ 9,\ 7,\ 2,\ 4) $ の部分列です。 - 全ての隣り合う要素の差の絶対値 ($ |1-4|,\ |4-3|,\ |3-6|,\ |6-9|,\ |9-7|,\ |7-4| $) は $ K\ =\ 3 $ 以下です。