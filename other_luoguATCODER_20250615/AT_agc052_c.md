# AT_agc052_c [AGC052C] Nondivisible Prefix Sums

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc052/tasks/agc052_c

素数 $ P $ が与えられます。これはあなたの嫌いな数です。

整数の列 $ A_1,\ A_2,\ \dots,\ A_N $ について、どの接頭辞の和も $ P $ で割り切れないように要素を並べ替えることができるとき、この列を **良い** 列と呼びます（すなわち、並べ替えのあと、$ 1\ \le\ i\ \le\ N $ かつ $ A_1\ +\ A_2\ +\ \dots\ +\ A_i\ \equiv\ 0\ \bmod\ P $ であるような $ i $ が **存在してはいけません**）。

各要素が $ 1 $ 以上 $ P-1 $ 以下であるような長さ $ N $ の整数列は全部で $ (P-1)^N $ 通りありますが、このうち **良い** 列はいくつでしょうか。

答えは非常に大きい可能性があるため、これを $ 998244353 $ で割った余りを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ P $

## 输出格式

**良い** 列の個数を $ 998244353 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 5
```

### 输出 #1

```
12
```

## 输入输出样例 #2

### 输入 #2

```
4 3
```

### 输出 #2

```
8
```

## 输入输出样例 #3

### 输入 #3

```
5000 99999989
```

### 输出 #3

```
51699346
```

## 输入输出样例 #4

### 输入 #4

```
2021 307
```

### 输出 #4

```
644635349
```

## 说明/提示

### 制約

- $ 1\ \le\ N\ \le\ 5000 $
- $ 2\ \le\ P\ \le\ 10^8 $
- $ P $ は素数である。

### Sample Explanation 1

良い列は $ [1,\ 1] $, $ [1,\ 2] $, $ [1,\ 3] $, $ [2,\ 1] $, $ [2,\ 2] $, $ [2,\ 4] $, $ [3,\ 1] $, $ [3,\ 3] $, $ [3,\ 4] $, $ [4,\ 2] $, $ [4,\ 3] $, $ [4,\ 4] $ の $ 12 $ 通りです。

### Sample Explanation 2

良い列は $ [1,\ 1,\ 1,\ 2] $, $ [1,\ 1,\ 2,\ 1] $, $ [1,\ 2,\ 1,\ 1] $, $ [2,\ 1,\ 1,\ 1] $, $ [2,\ 2,\ 2,\ 1 $\\\], $ [2,\ 2,\ 1,\ 2] $, $ [2,\ 1,\ 2,\ 2] $, $ [1,\ 2,\ 2,\ 2] $ の $ 8 $ 通りです。