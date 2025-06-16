# AT_abc287_e [ABC287E] Karuta

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc287/tasks/abc287_e

英小文字からなる文字列が $ N $ 個与えられます。$ i\ \,\ (i\ =\ 1,\ 2,\ \dots,\ N) $ 番目のものを $ S_i $ と表します。

二つの文字列 $ x,\ y $ に対し、以下の条件を全て満たす最大の整数 $ n $ を $ \mathrm{LCP}(x,\ y) $ と表します。

- $ x,\ y $ の長さはいずれも $ n $ 以上
- $ 1 $ 以上 $ n $ 以下の全ての整数 $ i $ に対し、$ x $ の $ i $ 文字目と $ y $ の $ i $ 文字目が等しい
 
全ての $ i\ =\ 1,\ 2,\ \dots,\ N $ に対し、以下の値を求めてください。

- $ \displaystyle\ \max_{i\ \neq\ j}\ \mathrm{LCP}(S_i,\ S_j) $

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式

$ N $ 行出力せよ。$ i\ \,\ (i\ =\ 1,\ 2,\ \dots,\ N) $ 行目には、$ \displaystyle\ \max_{i\ \neq\ j}\ \mathrm{LCP}(S_i,\ S_j) $ を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
abc
abb
aac
```

### 输出 #1

```
2
2
1
```

## 输入输出样例 #2

### 输入 #2

```
11
abracadabra
bracadabra
racadabra
acadabra
cadabra
adabra
dabra
abra
bra
ra
a
```

### 输出 #2

```
4
3
2
1
0
1
0
4
3
2
1
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 5\ \times\ 10^5 $
- $ N $ は整数
- $ S_i $ は英小文字からなる長さ $ 1 $ 以上の文字列 $ (i\ =\ 1,\ 2,\ \dots,\ N) $
- $ S_i $ の長さの総和は $ 5\ \times\ 10^5 $ 以下
 
### Sample Explanation 1

$ \mathrm{LCP}(S_1,\ S_2)\ =\ 2,\ \mathrm{LCP}(S_1,\ S_3)\ =\ 1,\ \mathrm{LCP}(S_2,\ S_3)\ =\ 1 $ です。