# AT_kupc2020_b Numbers on Papers

## 题目描述

[problemUrl]: https://atcoder.jp/contests/kupc2020/tasks/kupc2020_b

$ 1 $ から $ N $ までの番号が付けられた $ N $ 枚の紙があり、それぞれの紙には整数が $ K $ 個ずつ書かれています。

$ i $ 番目の紙に書いてある整数は $ v_{i,1},\ v_{i,2},\ \ldots\ v_{i,K} $ です。

それぞれの紙から独立に $ 1 $ つずつ整数を選び、$ i $ 番目の紙から選んだ整数が $ i $ 項目になるような数列を作ることを考えます。

このような数列の作り方は$ K^N $通りありますが、そのうち広義単調増加なものは何通りでしょうか？答えは非常に大きくなる可能性があるため、$ 10^9+7 $ で割ったあまりを求めてください。

ただし、数列 $ A=(a_1,\ a_2,\ \ldots\ ,\ a_N) $ が広義単調増加であるとは、全ての $ i\ (1\ \leq\ i\ \leq\ N-1) $ に対して $ a_i\ \leq\ a_{i+1} $ が成り立つことをいいます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ v_{1,1} $ $ v_{1,2} $ $ \cdots $ $ v_{1,K} $ $ v_{2,1} $ $ v_{2,2} $ $ \cdots $ $ v_{2,K} $ $ \vdots $ $ v_{N,1} $ $ v_{N,2} $ $ \cdots $ $ v_{N,K} $

## 输出格式

問題文で述べたような数列のうち、広義単調増加なものは何通りあるか、$ 10^9+7 $ で割ったあまりを一行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 2
2 4
1 5
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
2 3
4 5 6
1 2 3
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
20 20
2 8 12 17 19 29 41 53 57 62 63 65 67 70 71 74 76 77 96 100
2 3 9 13 15 16 20 26 28 33 38 39 46 51 58 59 74 92 93 99
2 5 6 9 19 20 22 24 26 35 41 45 56 60 62 74 76 81 83 96
3 7 10 11 13 15 17 20 22 26 34 35 43 59 68 78 82 83 85 93
1 7 11 14 17 26 37 41 45 49 62 63 64 67 71 74 88 89 91 94
12 15 17 19 22 24 28 29 31 46 50 51 55 59 64 65 74 79 91 95
7 11 17 22 23 27 29 33 37 39 45 50 51 52 62 67 69 71 85 90
9 11 12 18 22 30 40 41 43 49 51 59 62 71 74 94 95 96 99 100
15 17 21 23 24 28 33 39 44 45 48 52 54 59 72 76 88 89 99 100
1 6 12 13 14 21 25 37 48 49 56 57 71 72 77 79 83 85 93 98
10 20 22 25 34 45 49 52 58 60 62 67 69 74 75 77 81 84 96 97
6 7 23 36 41 43 45 46 50 51 52 57 58 61 73 74 85 87 94 97
4 20 26 36 37 41 44 45 47 51 56 57 72 73 74 79 86 91 97 98
8 10 17 24 25 29 31 32 34 46 53 57 60 71 74 78 79 80 90 91
12 15 16 17 27 32 33 35 41 51 55 56 58 67 69 71 74 89 90 91
4 13 17 24 25 27 39 40 43 48 51 54 61 62 63 68 72 76 87 90
8 10 12 18 22 37 40 43 46 50 51 58 59 65 74 85 86 89 96 98
1 9 16 17 19 34 37 50 54 55 57 58 59 69 72 76 77 84 92 99
3 10 11 12 13 17 24 28 36 39 45 49 50 58 74 78 79 80 84 93
5 15 16 20 22 24 29 41 44 55 56 60 62 63 68 73 85 86 93 100
```

### 输出 #3

```
188926982
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ 1\ \leq\ K\ \leq\ 10000 $
- $ 1\ \leq\ v_{i,1}\ <\ v_{i,2}\ <\ \cdots\ <\ v_{i,K}\ \leq\ 10^9\ (1\ \le\ i\ \le\ N) $
- 入力はすべて整数である。

### Sample Explanation 1

ありえる数列は以下の $ 4 $ つです。 - $ (2,1) $ - $ (2,5) $ - $ (4,1) $ - $ (4,5) $ このうち広義単調増加なものは $ (2,5) $ と $ (4,5) $ であるため、答えは $ 2 $ です。

### Sample Explanation 2

どのように整数を選んでも広義単調増加にできない場合もあります。

### Sample Explanation 3

$ 10^9+7 $ で割った余りを出力するように注意してください．