# AT_code_formula_2014_qualB_d お釣りの嫌いな高橋君

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-formula-2014-qualb/tasks/code_formula_2014_qualB_d

高橋君の国では、$ N $ 種類の硬貨が使われています。 $ 1 $ 番目の硬貨の価値は $ 1 $ 円です。 $ k $ 番目の硬貨の価値は、$ k-1 $ 番目の硬貨の $ 10 $ 倍あります。 つまり、$ 2 $ 番目の硬貨は $ 10 $ 円の価値があり、$ 5 $ 番目の硬貨は $ 10000 $ 円の価値があります。

高橋君は、お釣りが嫌いです。なので、出来るだけぴったりの金額で買い物がしたいと思っています。 そこで高橋君は、今持っている硬貨で、何種類の金額が払えるかを調べたいと思いました。

高橋君が払える金額が何通りあるかを出力しなさい。 ただし、これは膨大な数となるため、 $ 1000000007 $ 以上となる場合は、 $ 1000000007 $ で割った余りを出力しなさい。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ : $ A_N $

- $ 1 $ 行目には、硬貨の種類数 $ N\ (1\ ≦\ N\ ≦\ 50) $ が、$ 1 $ 行で与えられる。
- $ 2 $ 行目から $ N $ 行では、高橋君が各硬貨を何枚持っているかが与えられる。 このうち $ i(1≦i≦N) $ 行目では、 $ i $ 番目の硬貨を、高橋君が何枚持っているかを表す整数 $ A_i(0≦A_i≦50000) $が与えられる。

## 输出格式

高橋君が払える金額の種類数を、 $ 1000000007 $ で割った余りを $ 1 $ 行で出力せよ。出力の末尾は改行をいれること。

## 输入输出样例 #1

### 输入 #1

```
2
2
1
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
2
32
3
```

### 输出 #2

```
62
```

## 输入输出样例 #3

### 输入 #3

```
4
12
3
7
34
```

### 输出 #3

```
12039
```

## 输入输出样例 #4

### 输入 #4

```
10
1234
2
857
3858
1
5000
32
4
1
857
```

### 输出 #4

```
969347336
```

## 说明/提示

### Sample Explanation 1

払える金額は、$ 1 $ 円, $ 2 $ 円, $ 10 $ 円, $ 11 $ 円, $ 12 $ 円の $ 5 $ 通りとなります。 $ 0 $ 円は含まないことに注意してください。

### Sample Explanation 2

$ 1 $ 円から $ 62 $ 円の $ 62 $ 通りの金額を支払うことが出来ます。

### Sample Explanation 4

$ 1000000007 $ で割った余りを出力してください。