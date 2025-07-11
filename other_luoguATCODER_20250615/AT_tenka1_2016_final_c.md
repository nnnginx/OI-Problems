# AT_tenka1_2016_final_c たんごたくさん

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tenka1-2016-final/tasks/tenka1_2016_final_c

文字列 $ S $ と、要素数 $ M $ の単語の集合 $ P=\{P_1,\ P_2,\ …,\ P_M\} $ が与えられます。単語 $ P_i $ は、整数の重み $ W_i $ を持っています。

文字列 $ S $ から、$ P $ に含まれる単語を重なり合わないように取り出すことを考えます。単語の重みの総和が最大値をとるように取り出すとき、その最大値はいくつでしょうか？

なお、同じ単語を複数回取り出した場合、それらの単語は別々に数えることとします。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $ $ M $ $ P_1 $ : $ P_M $ $ W_1 $ : $ W_M $

## 输出格式

単語の重みの総和の最大値を $ 1 $ 行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
abcabcabc
3
ab
bc
ca
1
1
1
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
abracadabra
4
b
abra
cad
rac
1
10
50
100
```

### 输出 #2

```
111
```

## 输入输出样例 #3

### 输入 #3

```
abcd
2
ad
bc
1192
794
```

### 输出 #3

```
794
```

## 说明/提示

### 制約

- $ 1\ \leq\ |S|\ \leq\ 200000 $
- $ 1\ \leq\ M\ \leq\ 5000 $
- $ 1\ \leq\ |P_i|\ \leq\ 200 $
- $ 1\ \leq\ W_i\ \leq\ 10000 $
- $ S $, $ P_i $ は英小文字からなる文字列である