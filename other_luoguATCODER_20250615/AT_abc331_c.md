# AT_abc331_c [ABC331C] Sum of Numbers Greater Than Me

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc331/tasks/abc331_c

長さ $ N $ の数列 $ A=(A_1,\ldots,A_N) $ が与えられます。

$ i=1,\ldots,N $ のそれぞれについて次の問題を解いてください。

問題：$ A $ の要素のうち $ A_i $ より大きな要素全ての和を求めよ。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ \ldots $ $ A_N $

## 输出格式

各 $ 1\leq\ k\leq\ N $ について、$ i=k $ に対する問題の答えを $ B_k $ とする。$ B_1,\ldots,B_N $ をこの順に空白区切りで出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
1 4 1 4 2
```

### 输出 #1

```
10 0 10 0 8
```

## 输入输出样例 #2

### 输入 #2

```
10
31 42 59 26 53 58 97 93 23 54
```

### 输出 #2

```
456 414 190 487 361 249 0 97 513 307
```

## 输入输出样例 #3

### 输入 #3

```
50
1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1
```

### 输出 #3

```
0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0 0
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ 10^6 $
- 入力は全て整数である
 
### Sample Explanation 1

\- $ i=1 $ のとき $ A_1=1 $ より大きな要素の和は $ 4+4+2=10 $ - $ i=2 $ のとき $ A_2=4 $ より大きな要素の和は $ 0 $ - $ i=3 $ のとき $ A_3=1 $ より大きな要素の和は $ 4+4+2=10 $ - $ i=4 $ のとき $ A_4=4 $ より大きな要素の和は $ 0 $ - $ i=5 $ のとき $ A_5=2 $ より大きな要素の和は $ 4+4=8 $