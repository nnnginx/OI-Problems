# AT_yahoo_procon2017_qual_b オークション

## 题目描述

[problemUrl]: https://atcoder.jp/contests/yahoo-procon2017-qual/tasks/yahoo_procon2017_qual_b

高橋君はオークションサイトでの買い物を楽しんでいます。 今、このオークションサイトには $ N $ 個の商品が出品されており、$ i $ 個目の商品の値段は $ A_i $ 円です。 このオークションサイトでは、一日に一個までしか商品を買うことができず、 一日たつごとにどの商品も値段が $ 1 $ 円ずつ増えます。 もちろん、同じ商品は一度までしか買うことはできません。

高橋君は $ K $ 個の商品を買いたいです。 高橋君が $ K $ 個の商品を買うために必要な金額の最小値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ ... $ $ A_N $

## 输出格式

高橋君が $ K $ 個の商品を買うためにかかる金額の総和の最小値を一行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 2
1 3 5
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
5 3
6 3 2 4 7
```

### 输出 #2

```
12
```

## 说明/提示

### 制約

- $ 1\ ≦\ N\ ≦\ 10^5 $
- $ 1\ ≦\ K\ ≦\ N $
- $ 1\ ≦\ A_i\ ≦\ 10^9 $

### Sample Explanation 1

例えば、以下のように買い物をすれば高橋君は $ 5 $ 円で $ 2 $ 個の商品を買うことができます。 - $ 1 $ 日目に $ 3 $ 円の商品を買う。このとき、残りの商品の値段は $ 1 $ 円ずつ上がり、$ 2 $ 円と $ 6 $ 円の商品が残る。 - $ 2 $ 日目に $ 2 $ 円の商品を買う。このとき、使った金額の合計は $ 5 $ 円となる。