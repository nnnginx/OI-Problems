# AT_abc299_g [ABC299G] Minimum Permutation

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc299/tasks/abc299_g

$ 1 $ 以上 $ M $ 以下の整数からなる長さ $ N $ の数列 $ A $ があります。ここで、$ 1 $ 以上 $ M $ 以下のどの整数も $ A $ に $ 1 $ 回以上登場します。

$ A $ の長さ $ M $ の（連続とは限らない）部分列であって $ 1,\ \ldots,\ M $ が $ 1 $ 回ずつ登場するもののうち、辞書順最小のものを答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

求めるべき部分列を $ B_1,\ \ldots,\ B_M $ として、以下の形式で出力せよ。

> $ B_1 $ $ B_2 $ $ \ldots $ $ B_M $

## 输入输出样例 #1

### 输入 #1

```
4 3
2 3 1 3
```

### 输出 #1

```
2 1 3
```

## 输入输出样例 #2

### 输入 #2

```
4 4
2 3 1 4
```

### 输出 #2

```
2 3 1 4
```

## 输入输出样例 #3

### 输入 #3

```
20 10
6 3 8 5 8 10 9 3 6 1 8 3 3 7 4 7 2 7 8 5
```

### 输出 #3

```
3 5 8 10 9 6 1 4 2 7
```

## 说明/提示

### 制約

- $ 1\ \leq\ M\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ M $
- $ 1 $ 以上 $ M $ 以下のどの整数も $ A $ に $ 1 $ 回以上登場する。
- 入力中の値はすべて整数である。
 
### Sample Explanation 1

$ A $ の長さ $ 3 $ の部分列であって $ 1,\ 2,\ 3 $ が $ 1 $ 回ずつ登場するものは $ (2,\ 3,\ 1) $ と $ (2,\ 1,\ 3) $ であり、このうち辞書順で小さいのは $ (2,\ 1,\ 3) $ です。