# AT_agc010_d [AGC010D] Decrementing

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc010/tasks/agc010_d

黒板に $ N $ 個の整数が書かれています。$ i $ 番目の整数は $ A_i $ であり、これらの最大公約数は $ 1 $ です。

高橋君と青木君はこの数を使ってゲームをします。ゲームでは高橋君から始めて交互に以下の操作を繰り返します。

- 黒板の中から $ 2 $ 以上の数を $ 1 $ つ選び、その数から $ 1 $ を引く。
- その後、黒板に書かれた数の最大公約数を $ g $ として、すべての数を $ g $ で割る。

黒板に書かれた数が全て $ 1 $ となっていて、操作が行えない人の負けです。 二人が最適に行動したとき、どちらが勝つか求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ … $ A_N $

## 输出格式

先手の高橋君が勝つなら `First` を、後手の青木君が勝つなら `Second` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
3 6 7
```

### 输出 #1

```
First
```

## 输入输出样例 #2

### 输入 #2

```
4
1 2 4 8
```

### 输出 #2

```
First
```

## 输入输出样例 #3

### 输入 #3

```
5
7 8 8 8 8
```

### 输出 #3

```
Second
```

## 说明/提示

### 制約

- $ 1\ ≦\ N\ ≦\ 10^5 $
- $ 1\ ≦\ A_i\ ≦\ 10^9 $
- $ A_1 $ から $ A_N $ の最大公約数は $ 1 $

### Sample Explanation 1

以下のようにすれば先手の高橋君が勝てます。 - 高橋君が $ 7 $ から $ 1 $ を引く。このとき、操作後は $ (1,2,2) $ となる。 - 青木君が $ 2 $ から $ 1 $ を引く。このとき、操作後は $ (1,1,2) $ となる。 - 高橋君が $ 2 $ から $ 1 $ を引く。このとき、操作後は $ (1,1,1) $ となる。