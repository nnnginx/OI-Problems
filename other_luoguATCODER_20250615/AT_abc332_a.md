# AT_abc332_a [ABC332A] Online Shopping

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc332/tasks/abc332_a

AtCoder 社は、[オンラインショップ](https://suzuri.jp/AtCoder/home)でグッズを販売しています。

高橋君はそこで $ N $ 種類の商品を購入することにしました。  
$ 1 $ 以上 $ N $ 以下の整数 $ i $ について、$ i $ 種類目の商品は $ 1 $ 個 $ P_i $ 円で、高橋君は $ Q_i $ 個購入します。

また、高橋君は送料を支払う必要があります。  
送料は購入する商品の合計金額が $ S $ 円以上なら $ 0 $ 円、そうでないならば $ K $ 円です。

高橋君が支払う金額は購入する商品の合計金額と送料の和です。  
高橋君が支払う金額を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $ $ K $ $ P_1 $ $ Q_1 $ $ P_2 $ $ Q_2 $ $ \vdots $ $ P_N $ $ Q_N $

## 输出格式

高橋君がオンラインショッピングで支払う金額を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 2000 500
1000 1
100 6
```

### 输出 #1

```
2100
```

## 输入输出样例 #2

### 输入 #2

```
3 2000 500
1000 1
100 6
5000 1
```

### 输出 #2

```
6600
```

## 输入输出样例 #3

### 输入 #3

```
2 2000 500
1000 1
1000 1
```

### 输出 #3

```
2000
```

## 说明/提示

### 制約

- $ 1\leq\ N\leq\ 100 $
- $ 1\leq\ S\leq\ 10000 $
- $ 1\leq\ K\leq\ 10000 $
- $ 1\leq\ P_i\leq\ 10000 $
- $ 1\leq\ Q_i\leq\ 100 $
- 入力はすべて整数

### Sample Explanation 1

高橋君は $ 1 $ 個 $ 1000 $ 円の商品を $ 1 $ 個と、 $ 1 $ 個 $ 100 $ 円の商品を $ 6 $ つ購入します。 よって、購入する商品の合計金額は $ 1000\times\ 1+100\times\ 6=1600 $ 円となります。 このとき購入する商品の合計金額は $ 2000 $ 円未満であるため、送料は $ 500 $ 円となります。 よって、高橋君の支払う金額は $ 1600+500=2100 $ 円となります。

### Sample Explanation 2

購入する商品の合計金額は $ 1000\times\ 1+100\times\ 6＋5000\times\ 1=6600 $ 円となります。 このとき購入する商品の合計金額は $ 2000 $ 円以上であるため、送料は $ 0 $ 円となります。 よって、高橋君の支払う金額は $ 6600+0=6600 $ 円となります。

### Sample Explanation 3

$ 1 $ 個あたりの価格が同じ商品が複数存在することもあります。