## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc282/tasks/abc282_h

$ 2 $ つの長さ $ N $ の整数列 $ A\ =\ (A_1,\ A_2,\ \ldots,\ A_N) $ および $ B\ =\ (B_1,\ B_2,\ \ldots,\ B_N) $ が与えられます。

$ 1\ \leq\ l\ \leq\ r\ \leq\ N $ を満たす整数の組 $ (l,\ r) $ であって下記の条件を満たすものの個数を出力してください。

- $ \min\lbrace\ A_l,\ A_{l+1},\ \ldots,\ A_r\ \rbrace\ +\ (B_l\ +\ B_{l+1}\ +\ \cdots\ +\ B_r)\ \leq\ S $

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $ $ B_1 $ $ B_2 $ $ \ldots $ $ B_N $

## 输出格式
答えを出力せよ。

## 题目大意
给定序列 $A,B$，求有多少对 $(l,r)$ 满足 $1\le l\le r\le n$，且 
$$
\sum_{i=l}^rB_i+\min_{i=l}^rA_i\le S
$$

```input1
4 15
9 2 6 5
3 5 8 9
```

```output1
6
```

```input2
15 100
39 9 36 94 40 26 12 26 28 66 73 85 62 5 20
0 0 7 7 0 5 5 0 7 9 9 4 2 5 2
```

```output2
119
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 0\ \leq\ S\ \leq\ 3\ \times\ 10^{14} $
- $ 0\ \leq\ A_i\ \leq\ 10^{14} $
- $ 0\ \leq\ B_i\ \leq\ 10^9 $
- 入力はすべて整数
 
### Sample Explanation 1

$ 1\ \leq\ l\ \leq\ r\ \leq\ N $ を満たす整数の組 $ (l,\ r) $ であって問題文中の条件を満たすものは、 $ (1,\ 1),\ (1,\ 2),\ (2,\ 2),\ (2,\ 3),\ (3,\ 3),\ (4,\ 4) $ の $ 6 $ 個です。

