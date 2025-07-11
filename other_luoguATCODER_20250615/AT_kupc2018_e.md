# AT_kupc2018_e 転倒数

## 题目描述

[problemUrl]: https://atcoder.jp/contests/kupc2018/tasks/kupc2018_e

長さ $ N $ の順列 $ P\ =\ p_1,\ p_2,\ ...,\ p_N $ が与えられます。長さ $ N $ の順列であって、$ P $ より辞書順で小さいか等しいもの全てについて転倒数を求め、その和を答えてください。ただし答えはとても大きくなることがあるので、$ 10^9\ +\ 7 $ で割った余りを出力してください。

ただし、順列 $ X\ =\ x_1,\ x_2,\ ...,\ x_N $ の転倒数とは、$ 1\ \leq\ i\ <\ j\ \leq\ N $ かつ $ x_i\ >\ x_j $ を満たす整数 $ i,\ j $ の組の個数のことです。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ p_1 $ $ p_2 $ $ ... $ $ p_N $

## 输出格式

長さ $ N $ の順列であって、順列 $ P $ より辞書順で小さいか等しいもの全てについて転倒数を求め、その和を $ 10^9\ +\ 7 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
2 1 3
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
4
1 2 3 4
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
8
5 6 2 7 1 3 8 4
```

### 输出 #3

```
281881
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ p_i\ \leq\ N $
- 入力は全て整数である。
- $ p_1,\ p_2,\ ...,\ p_N $ は順列である。

### Sample Explanation 1

順列 $ (2,\ 1,\ 3) $ より辞書順で小さいか等しい、長さ $ 3 $ の順列は $ (1,\ 2,\ 3) $, $ (1,\ 3,\ 2) $, $ (2,\ 1,\ 3) $ の $ 3 $ 種類です。 これらの順列の転倒数はそれぞれ $ 0,\ 1,\ 1 $ なので、答えは $ 0\ +\ 1\ +\ 1\ =\ 2 $ となります。