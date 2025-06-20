# AT_abc367_g [ABC367G] Sum of (XOR^K or 0)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc367/tasks/abc367_g

正整数 $ N,M,K $ および非負整数列 $ A=(A_1,A_2,\ldots,A_N) $ が与えられます。

非空な非負整数列 $ B=(B_1,B_2,\ldots,B_{|B|}) $ に対して、**スコア**を以下で定めます。

- $ B $ の長さが $ M $ の倍数のとき $ (B_1\ \oplus\ B_2\ \oplus\ \dots\ \oplus\ B_{|B|})^K $
- そうでないとき $ 0 $
 
ただし、$ \oplus $ はビットごとの排他的論理和を表します。

$ A $ の非空な部分列 $ 2^N-1 $ 個それぞれに対するスコアの総和を $ 998244353 $ で割った余りを求めてください。

 ビットごとの排他的論理和とは 非負整数 $ A,\ B $ のビットごとの排他的論理和 $ A\ \oplus\ B $ は、以下のように定義されます。 - $ A\ \oplus\ B $ を二進表記した際の $ 2^k $ ($ k\ \geq\ 0 $) の位の数は、$ A,\ B $ を二進表記した際の $ 2^k $ の位の数のうち一方のみが $ 1 $ であれば $ 1 $、そうでなければ $ 0 $ である。

 例えば、$ 3\ \oplus\ 5\ =\ 6 $ となります (二進表記すると: $ 011\ \oplus\ 101\ =\ 110 $)。  
 一般に $ k $ 個の整数 $ p_1,\ \dots,\ p_k $ の排他的論理和は $ (\cdots\ ((p_1\ \oplus\ p_2)\ \oplus\ p_3)\ \oplus\ \cdots\ \oplus\ p_k) $ と定義され、これは $ p_1,\ \dots,\ p_k $ の順番によらないことが証明できます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ K $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 2 2
1 2 3
```

### 输出 #1

```
14
```

## 输入输出样例 #2

### 输入 #2

```
10 5 3
100 100 100 100 100 100 100 100 100 100
```

### 输出 #2

```
252000000
```

## 输入输出样例 #3

### 输入 #3

```
16 4 100
7053 3876 3178 8422 7802 5998 2334 6757 6889 6637 7365 9495 7848 9026 7312 6558
```

### 输出 #3

```
432440016
```

## 说明/提示

### 制約

- $ 1\leq\ N,K\leq\ 2\times\ 10^5 $
- $ 1\leq\ M\leq\ 100 $
- $ 0\leq\ A_i\lt\ 2^{20} $
- 入力は全て整数
 
### Sample Explanation 1

$ A $ の非空な部分列 $ 2^3-1=7 $ 個それぞれのスコアは以下のようになります。 - $ (1) $：$ 0 $ - $ (2) $：$ 0 $ - $ (3) $：$ 0 $ - $ (1,2) $：$ (1\oplus2)^2=9 $ - $ (1,3) $：$ (1\oplus3)^2=4 $ - $ (2,3) $：$ (2\oplus3)^2=1 $ - $ (1,2,3) $：$ 0 $ よって求める総和は $ 0+0+0+9+4+1+0=14 $ です。