# AT_abc159_d [ABC159D] Banned K

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc159/tasks/abc159_d

ボールが $ N $ 個あり、 $ i $ 番目のボールには整数 $ A_i $ が書かれています。  
 $ k=1,2,...,N $ に対して以下の問題を解いて、答えをそれぞれ出力してください。

- $ k $ 番目のボールを除いた $ N-1 $ 個のボールから、書かれている整数が等しいような異なる $ 2 $ つのボールを選び出す方法の数を求めてください。選ぶ順序は考慮しません。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ ... $ $ A_N $

## 输出格式

$ k=1,2,...,N $ に対する答えを順番に一行ずつ出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
1 1 2 1 2
```

### 输出 #1

```
2
2
3
2
3
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
0
0
0
```

## 输入输出样例 #3

### 输入 #3

```
5
3 3 3 3 3
```

### 输出 #3

```
6
6
6
6
6
```

## 输入输出样例 #4

### 输入 #4

```
8
1 2 1 4 2 1 4 1
```

### 输出 #4

```
5
7
5
7
7
5
7
5
```

## 说明/提示

### 制約

- $ 3\ \leq\ N\ \leq\ 2\ \times\ 10^5 $
- $ 1\ \leq\ A_i\ \leq\ N $
- 入力はすべて整数である。

### Sample Explanation 1

例えば $ k=1 $ のとき、残りのボールに書かれている数はそれぞれ $ {1,2,1,2} $ です。 この中から書かれている数が等しいような異なる $ 2 $ つのボールを選び出す方法は $ 2 $ 通りあります。 したがって、 $ k=1 $ に対する問題の答えは $ 2 $ です。

### Sample Explanation 2

どの $ 2 $ つのボールを選び出しても、書かれている数は等しくありません。

### Sample Explanation 3

どの $ 2 $ つのボールを選び出しても、書かれている数が等しいです。