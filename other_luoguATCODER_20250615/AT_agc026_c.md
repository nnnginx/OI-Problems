# AT_agc026_c [AGC026C] String Coloring

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc026/tasks/agc026_c

長さ $ 2N $ の，英小文字のみからなる文字列 $ S $ が与えられます。

$ S $ の各文字を赤色か青色かに塗り分ける方法は $ 2^{2N} $ 通りありますが，このうち以下の条件を満たす塗り分け方は何通りですか？

- 赤色に塗られた文字を**左から右に**読んだ文字列と，青色に塗られた文字を**右から左に**読んだ文字列が一致する

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式

条件を満たす塗り分け方の個数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
cabaacba
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
11
mippiisssisssiipsspiim
```

### 输出 #2

```
504
```

## 输入输出样例 #3

### 输入 #3

```
4
abcdefgh
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
18
aaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
```

### 输出 #4

```
9075135300
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 18 $
- $ S $ の長さは $ 2N $ である
- $ S $ は英小文字のみからなる

### Sample Explanation 1

以下の $ 4 $ 通りの塗り分け方が存在します。 - cabaacba - cabaacba - cabaacba - cabaacba

### Sample Explanation 4

答えは32bit整数型で表せないこともあります。