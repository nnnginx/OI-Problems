# AT_abc250_d [ABC250D] 250-like Number

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc250/tasks/abc250_d

以下の条件を満たす整数 $ k $ を「 $ 250 $ に似た数」と呼びます。

- $ k $ が素数 $ p\ <\ q $ を使って $ k=p\ \times\ q^3 $ と表される。

$ N $ 以下の「 $ 250 $ に似た数」は全部でいくつありますか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式

答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
250
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
1
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
123456789012345
```

### 输出 #3

```
226863
```

## 说明/提示

### 制約

- $ N $ は $ 1 $ 以上 $ 10^{18} $ 以下の整数

### Sample Explanation 1

\- $ 54\ =\ 2\ \times\ 3^3 $ なので、「 $ 250 $ に似た数」です。 - $ 250\ =\ 2\ \times\ 5^3 $ なので、「 $ 250 $ に似た数」です。 $ 250 $ 以下の「 $ 250 $ に似た数」は、以上の $ 2 $ つです。