# AT_abc084_d [ABC084D] 2017-like Number

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc084/tasks/abc084_d

「$ N $ も $ (N+1)÷2 $ も素数」を満たす奇数 $ N $ を **2017に似た数** とします。

$ Q $ 個のクエリが与えられます。

クエリ $ i(1≦i≦Q) $ では奇数 $ l_i $,$ r_i $ が与えられるので、$ l_i≦x≦r_i $ かつ **2017に似た数** となる奇数 $ x $ の個数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ Q $ $ l_1 $ $ r_1 $ $ : $ $ l_Q $ $ r_Q $

## 输出格式

$ i $ 行目 $ (1≦i≦Q) $ に、クエリ $ i $ の答えが $ x $ 個のとき、$ x $ を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1
3 7
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
4
13 13
7 11
7 11
2017 2017
```

### 输出 #2

```
1
0
0
1
```

## 输入输出样例 #3

### 输入 #3

```
6
1 53
13 91
37 55
19 51
73 91
13 49
```

### 输出 #3

```
4
4
1
1
1
2
```

## 说明/提示

### 制約

- $ 1≦Q≦10^5 $
- $ 1≦l_i≦r_i≦10^5 $
- $ l_i $,$ r_i $ は奇数
- 入力は全て整数

### Sample Explanation 1

\- $ 3 $ も $ (3+1)÷2=2 $ も素数であるため、$ 3 $ は \*\*2017に似た数\*\* です。 - $ 5 $ も $ (5+1)÷2=3 $ も素数であるため、$ 5 $ は \*\*2017に似た数\*\* です。 - $ 7 $ は素数ですが、 $ (7+1)÷2=4 $ は素数ではないため、$ 7 $ は \*\*2017に似た数\*\* ではありません。 よって、クエリ $ 1 $ の答えは $ 2 $ 個です。

### Sample Explanation 2

$ 2017 $ も \*\*2017に似た数\*\* であることに注意してください。