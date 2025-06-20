# AT_arc040_c [ARC040C] Z塗り

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc040/tasks/arc040_c

イカの高橋君は床を塗るのが大好きです。床は $ N\ \times\ N $ のマス目状に区切られており、すでにいくつかのマスは塗られています。$ i $ 行目 $ j $ 列目のマスをマス $ (i,j) $ と呼ぶことにします。高橋君は特殊なインク発射装置を用いて床を塗ろうとしています。この装置を使うと、以下のように床を塗ることができます。

- 任意の整数 $ r,\ c $ を入力して装置のボタンを押すと、「$ i\ =\ r $ かつ $ j\ ≦\ c $」または「$ i\ =\ r+1 $ かつ $ j\ ≧\ c $」を満たすようなすべてのマス $ (i,j) $ を塗ることができる。

高橋君は、全てのマスをこの装置で塗ろうと思っています。このとき、装置を使う必要のある回数の最小値を求めてください。

## 输入格式

入力はイカの形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ : $ S_N $

- $ 1 $ 行目には、マス目の $ 1 $ 辺の個数を表す整数 $ N\ (1\ ≦\ N\ ≦\ 100) $ が与えられる。
- $ 2 $ 行目からの $ N $ 行には、マス目の情報が与えられる。このうち $ i\ (1\ ≦\ i\ ≦\ N) $ 行目には、長さ $ N $ の文字列 $ S_i $ が与えられる。このうち $ j\ (1\ ≦\ j\ ≦\ N) $ 文字目は、マス $ (i,j) $ の情報を以下のように表す。 
  - `.` の場合：このマスがまだ塗られていないことを表す。
  - `o` の場合：このマスがすでに塗られていることを表す。

## 输出格式

装置を使う回数の最小値を $ 1 $ 行に出力せよ。出力の末尾に改行を入れること。

## 输入输出样例 #1

### 输入 #1

```
7
...oooo
oo.....
ooooooo
ooooooo
.....oo
oooo...
ooooooo
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
4
.oo.
..oo
o..o
oo..
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
1
o
```

### 输出 #3

```
0
```

## 说明/提示

### Sample Explanation 1

インク発射装置はこの入力のような形を綺麗に塗ることができます。

### Sample Explanation 3

はじめから全て塗られていることもあります。