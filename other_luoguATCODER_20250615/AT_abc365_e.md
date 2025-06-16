# AT_abc365_e [ABC365E] Xor Sigma Problem

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc365/tasks/abc365_e

長さ $ N $ の整数列 $ A=(A_1,\ldots,A_N) $ が与えられます。次の式の値を求めてください。

$ \displaystyle\ \sum_{i=1}^{N-1}\sum_{j=i+1}^N\ (A_i\ \oplus\ A_{i+1}\oplus\ \ldots\ \oplus\ A_j) $

 ビット単位 xor とは 非負整数 $ A,\ B $ のビット単位 xor 、$ A\ \oplus\ B $ は、以下のように定義されます。 - $ A\ \oplus\ B $ を二進表記した際の $ 2^k $ ($ k\ \geq\ 0 $) の位の数は、$ A,\ B $ を二進表記した際の $ 2^k $ の位の数のうち一方のみが $ 1 $ であれば $ 1 $、そうでなければ $ 0 $ である。

 例えば、$ 3\ \oplus\ 5\ =\ 6 $ となります (二進表記すると: $ 011\ \oplus\ 101\ =\ 110 $)。  
 一般に $ k $ 個の整数 $ p_1,\ \dots,\ p_k $ の排他的論理和は $ (\cdots\ ((p_1\ \oplus\ p_2)\ \oplus\ p_3)\ \oplus\ \cdots\ \oplus\ p_k) $ と定義され、これは $ p_1,\ \dots,\ p_k $ の順番によらないことが証明できます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_{N} $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
1 3 2
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
7
2 5 6 5 2 1 7
```

### 输出 #2

```
83
```

## 说明/提示

### 制約

- $ 2\leq\ N\leq\ 2\times\ 10^5 $
- $ 1\leq\ A_i\ \leq\ 10^8 $
- 入力される数値は全て整数
 
### Sample Explanation 1

$ A_1\oplus\ A_2\ =\ 2,\ A_1\ \oplus\ A_2\oplus\ A_3\ =\ 0,\ A_2\oplus\ A_3\ =\ 1 $ なので答えは $ 2+0+1=3 $ です。