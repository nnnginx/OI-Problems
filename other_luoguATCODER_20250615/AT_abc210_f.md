# AT_abc210_f [ABC210F] Coprime Solitaire

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc210/tasks/abc210_f

テーブルの上に $ N $ 枚のカードが並んでいます。 $ i\ =\ 1,\ 2,\ \ldots,\ N $ について、$ i $ 枚目のカードの表には整数 $ A_i $ が、裏には整数 $ B_i $ が書かれています。  
 はじめ、すべてのカードは表が見えるように置かれています。

高橋君は好きな枚数（ $ 0 $ 枚でも良い）のカードを選んで裏返します。 その結果、以下の条件が満たされれば高橋君はうれしい気持ちになります。

- $ 1\ \leq\ i\ \lt\ j\ \leq\ N $ を満たす任意の整数のペア $ (i,\ j) $ について、$ i $ 枚目のカードの見えている面に書かれた整数と、$ j $ 枚目のカードの見えている面に書かれた整数が、互いに素である。

高橋君がうれしい気持ちになれる可能性があるかどうかを判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ B_1 $ $ A_2 $ $ B_2 $ $ \vdots $ $ A_N $ $ B_N $

## 输出格式

高橋君がうれしい気持ちになれる可能性があるなら `Yes` を、可能性がないなら `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
2 5
10 9
4 8
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
2
10 100
1000 10000
```

### 输出 #2

```
No
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 3\ \times\ 10^4 $
- $ 1\ \leq\ A_i,\ B_i\ \leq\ 2\ \times\ 10^6 $
- 入力はすべて整数

### Sample Explanation 1

はじめ、見えている整数は $ 2,\ 10,\ 4 $ です。 $ 1 $ 枚目のカードと $ 2 $ 枚目のカードを裏返すと、見えている整数は $ 5,\ 9,\ 4 $ となり、高橋君はうれしい気持ちになります。よって `Yes` を出力します。

### Sample Explanation 2

どのようにカードを裏返しても、高橋君はうれしい気持ちになりません。よって `No` を出力します。