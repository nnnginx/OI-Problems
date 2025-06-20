# AT_abc119_c [ABC119C] Synthetic Kadomatsu

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc119/tasks/abc119_c

あなたは $ N $ 本の竹を持っています。これらの長さはそれぞれ $ l_1,\ l_2,\ ...,\ l_N $ です (単位: センチメートル)。

あなたの目的は、これらの竹のうち何本か (全部でもよい) を使い、長さが $ A,\ B,\ C $ であるような $ 3 $ 本の竹を得ることです。そのために、以下の三種類の魔法を任意の順に何度でも使うことができます。

- 延長魔法: $ 1 $ *MP* (マジックポイント) を消費し、$ 1 $ 本の竹を選んでその長さを $ 1 $ 増やす。
- 短縮魔法: $ 1 $ MP を消費し、$ 1 $ 本の長さ $ 2 $ 以上の竹を選んでその長さを $ 1 $ 減らす。
- 合成魔法: $ 10 $ MP を消費し、$ 2 $ 本の竹を選んで接続し $ 1 $ 本の竹とする。この新たな竹の長さは接続した $ 2 $ 本の竹の長さの合計に等しい。(以後、この竹に対してさらに魔法を使用することもできる。)

目的を達成するには、最小でいくつの MP が必要でしょうか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A $ $ B $ $ C $ $ l_1 $ $ l_2 $ $ : $ $ l_N $

## 输出格式

目的の達成に必要な MP の最小量を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 100 90 80
98
40
30
21
80
```

### 输出 #1

```
23
```

## 输入输出样例 #2

### 输入 #2

```
8 100 90 80
100
100
90
90
90
80
80
80
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
8 1000 800 100
300
333
400
444
500
555
600
666
```

### 输出 #3

```
243
```

## 说明/提示

### 制約

- $ 3\ \leq\ N\ \leq\ 8 $
- $ 1\ \leq\ C\ <\ B\ <\ A\ \leq\ 1000 $
- $ 1\ \leq\ l_i\ \leq\ 1000 $
- 入力される値はすべて整数である。

### Sample Explanation 1

長さ $ 98,\ 40,\ 30,\ 21,\ 80 $ の $ 5 $ 本の竹から長さ $ 100,\ 90,\ 80 $ の $ 3 $ 本の竹を得ようとしています。長さ $ 80 $ の竹ははじめから持っており、長さ $ 100,\ 90 $ の竹は次のように魔法を使うと合計 $ 23 $ MP を消費することで得られ、これが最適です。 1. 長さ $ 98 $ の竹に延長魔法を $ 2 $ 回使い、長さ $ 100 $ の竹を得る。(消費 MP: $ 2 $) 2. 長さ $ 40,\ 30 $ の竹に合成魔法を使い、長さ $ 70 $ の竹を得る。(消費 MP: $ 10 $) 3. 長さ $ 21 $ の竹に短縮魔法を $ 1 $ 回使い、長さ $ 20 $ の竹を得る。(消費 MP: $ 1 $) 4. 手順 2. で得た長さ $ 70 $ の竹と手順 3. で得た長さ $ 20 $ の竹に合成魔法を使い、長さ $ 90 $ の竹を得る。(消費 MP: $ 10 $)

### Sample Explanation 2

欲しい長さの竹をすでにすべて持っている場合、必要な MP は $ 0 $ です。このように、必ずしもすべての竹を使う必要はありません。