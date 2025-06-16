# AT_abc201_b [ABC201B] Do you know the second highest mountain?

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc201/tasks/abc201_b

AtCoder国には $ N $ 個の山があり、$ i $ 個目の山の名前は $ S_i $, 高さは $ T_i $ です。

$ 2 $ 番目に高い山の名前を答えてください。$ N $ 個の山の名前、高さはそれぞれ相異なることが保証されます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ T_1 $ $ S_2 $ $ T_2 $ $ \vdots $ $ S_N $ $ T_N $

## 输出格式

$ 2 $ 番目に高い山の名前を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
Everest 8849
K2 8611
Kangchenjunga 8586
```

### 输出 #1

```
K2
```

## 输入输出样例 #2

### 输入 #2

```
4
Kita 3193
Aino 3189
Fuji 3776
Okuhotaka 3190
```

### 输出 #2

```
Kita
```

## 输入输出样例 #3

### 输入 #3

```
4
QCFium 2846
chokudai 2992
kyoprofriends 2432
penguinman 2390
```

### 输出 #3

```
QCFium
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 1000 $
- $ 1\ \leq\ (S_i $ の長さ$ {})\ \leq\ 15 $
- $ 1\ \leq\ T_i\ \leq\ 10^5 $
- $ S_i\ \neq\ S_j\ (i\ \neq\ j) $
- $ T_i\ \neq\ T_j\ (i\ \neq\ j) $
- $ S_i $ は英小文字、英大文字、数字のみからなる
- $ N,\ T_i $ は整数

### Sample Explanation 1

世界で $ 2 $ 番目に高い山は K2 です。

### Sample Explanation 2

日本で $ 2 $ 番目に高い山は北岳です。