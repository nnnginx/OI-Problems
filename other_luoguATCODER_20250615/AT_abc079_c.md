# AT_abc079_c [ABC079C] Train Ticket

## 题目背景

有四个0到9之间的数字ABCD，在公式A op1 B op2 C op3 D = 7中，将符号op1、op2和op3中的每一个替换为+或-以便公式成立。保证有方案成立。输出任意一种方案

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc079/tasks/abc079_c

駅の待合室に座っているjoisinoお姉ちゃんは、切符を眺めています。

切符には $ 4 $ つの $ 0 $ 以上 $ 9 $ 以下の整数 $ A $,$ B $,$ C $,$ D $ が整理番号としてこの順に書かれています。

$ A $ $ op1 $ $ B $ $ op2 $ $ C $ $ op3 $ $ D $ $ = $ $ 7 $ となるように、$ op1 $,$ op2 $,$ op3 $ に `+` か `-` を入れて式を作って下さい。

なお、答えが存在しない入力は与えられず、また答えが複数存在する場合はどれを出力してもよいものとします。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ ABCD $

## 输出格式

作った式を、`=7` の部分を含めて出力せよ。

ただし、記号は半角で出力せよ。

また、数字と記号の間に空白を入れてはならない。

## 输入输出样例 #1

### 输入 #1

```
1222
```

### 输出 #1

```
1+2+2+2=7
```

## 输入输出样例 #2

### 输入 #2

```
0290
```

### 输出 #2

```
0-2+9+0=7
```

## 输入输出样例 #3

### 输入 #3

```
3242
```

### 输出 #3

```
3+2+4-2=7
```

## 说明/提示

### 制約

- $ 0≦A,B,C,D≦9 $
- 入力は整数からなる
- 答えが存在しない入力は与えられない

### Sample Explanation 1

$ 1\ +\ 2\ +\ 2\ +\ 2\ =\ 7 $ が条件を満たします。

### Sample Explanation 2

この他に、$ 0\ -\ 2\ +\ 9\ -\ 0\ =\ 7 $ が条件を満たします。