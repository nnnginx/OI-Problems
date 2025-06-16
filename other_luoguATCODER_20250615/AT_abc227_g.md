# AT_abc227_g [ABC227G] Divisors of Binomial Coefficient

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc227/tasks/abc227_g

二項係数 $ \displaystyle\ \binom{N}{K} $ の正の約数の個数を $ 998244353 $ で割った余りを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 2
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
103 3
```

### 输出 #2

```
8
```

## 输入输出样例 #3

### 输入 #3

```
1000000000000 1000000
```

### 输出 #3

```
110520107
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^{12} $
- $ 0\ \leq\ K\ \leq\ \min(10^6,N) $
- 入力に含まれる値は全て整数である

### Sample Explanation 1

$ \displaystyle\ \binom{5}{2}=10 $ です。$ 10 $ の正の約数は $ 1,2,5,10 $ の $ 4 $ 個です。

### Sample Explanation 2

$ \displaystyle\ \binom{103}{3}=176851 $ です。$ 176851 $ の正の約数は $ 8 $ 個あります。