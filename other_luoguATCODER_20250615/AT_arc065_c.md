# AT_arc065_c [ARC065E] へんなコンパス

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc065/tasks/arc065_c

$ xy $ 平面上に $ N $ 個の穴があります。$ i $ 番目の穴の位置は $ (x_i,y_i) $ です。

$ i $ 番目の穴と $ j $ 番目の穴のマンハッタン距離を $ d(i,j)(=|x_i-x_j|+|y_i-y_j|) $ と表します。

あなたはマンハッタンコンパスを持っています。 このコンパスは、常に $ 2 $ 個の穴を指します。 コンパスが $ p,\ q $ 番目の穴を指している状態と、$ q,\ p $ 番目の穴を指している状態は区別しません。

また、$ d(p,q)=d(p,r) $ で、$ p $ 番目の穴と $ q $ 番目の穴を指しているとき、$ p $ 番目の穴と $ r $ 番目の穴を指すよう動かすことができます。

はじめ、コンパスは $ a $ 番目の穴と $ b $ 番目の穴を指しています。 コンパスが指すことのできる穴の組の数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ a $ $ b $ $ x_1 $ $ y_1 $ : $ x_N $ $ y_N $

## 输出格式

コンパスが指すことのできる穴の組の数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 1 2
1 1
4 3
6 1
5 5
4 8
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
6 2 3
1 3
5 3
3 5
8 4
4 7
2 5
```

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
8 1 2
1 5
4 3
8 2
4 7
8 8
3 3
6 6
4 8
```

### 输出 #3

```
7
```

## 说明/提示

### 制約

- $ 2≦N≦10^5 $
- $ 1≦x_i,\ y_i≦10^9 $
- $ 1≦a\ <\ b≦N $
- $ i\ ≠\ j $ のとき $ (x_i,\ y_i)\ ≠\ (x_j,\ y_j) $
- $ x_i,\ y_i $ は整数である

### Sample Explanation 1

はじめ、コンパスは 穴 $ 1,\ 2 $ を指しています。 $ d(1,2)\ =\ d(1,3) $ なので、穴 $ 1,\ 3 $を指すことができます。 $ d(1,3)\ =\ d(3,4) $ なので、穴 $ 3,\ 4 $を指すことができます。 $ d(1,2)\ =\ d(2,5) $ なので、穴 $ 2,\ 5 $を指すことができます。 他の穴の組でコンパスが指せるものはないため、答えは $ 4 $ となります。