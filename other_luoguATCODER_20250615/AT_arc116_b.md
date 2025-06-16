# AT_arc116_b [ARC116B] Products of Min-Max

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc116/tasks/arc116_b

長さ $ N $ の整数列 $ A $ が与えられます。$ A $ の空でない部分列 $ B $ は $ 2^N\ -\ 1 $ 個あります。これらについて $ \max\left(B\right)\ \times\ \min\left(B\right) $ の値を計算し、その総和を答えてください。

ただし、答えは非常に大きくなる場合があるので、 $ 998244353 $ で割った余りを答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
2 4 3
```

### 输出 #1

```
63
```

## 输入输出样例 #2

### 输入 #2

```
1
10
```

### 输出 #2

```
100
```

## 输入输出样例 #3

### 输入 #3

```
7
853983 14095 543053 143209 4324 524361 45154
```

### 输出 #3

```
206521341
```

## 说明/提示

### 制約

- 入力は全て整数
- $ 1\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 0\ \leq\ A_i\ \leq\ 998244352 $

### Sample Explanation 1

$ B $ として、以下の $ 7 $ つが考えられます。 - $ B\ =\ \left(2\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 4 $ - $ B\ =\ \left(4\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 16 $ - $ B\ =\ \left(3\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 9 $ - $ B\ =\ \left(2,\ 4\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 8 $ - $ B\ =\ \left(2,\ 3\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 6 $ - $ B\ =\ \left(4,\ 3\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 12 $ - $ B\ =\ \left(2,\ 4,\ 3\right) $ : $ \max\left(B\right)\ \times\ \min\left(B\right)\ =\ 8 $ 以上の $ 7 $ つの値を足した値 $ 63 $ が答えです。