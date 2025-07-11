# AT_abc128_b [ABC128B] Guidebook

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc128/tasks/abc128_b

あなたは美味しいレストランを紹介する本を書くことにしました。 あなたは $ N $ 個のレストラン、レストラン $ 1 $、レストラン $ 2 $、$ … $、レストラン $ N $ を紹介しようとしています。レストラン $ i $ は $ S_i $ 市にあり、あなたは $ 100 $ 点満点中 $ P_i $ 点と評価しています。 異なる $ 2 $ 個のレストランに同じ点数がついていることはありません。

この本では、次のような順でレストランを紹介しようとしています。

- 市名が辞書順で早いものから紹介していく。
- 同じ市に複数レストランがある場合は、点数が高いものから紹介していく。

この本で紹介される順にレストランの番号を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ P_1 $ $ : $ $ S_N $ $ P_N $

## 输出格式

$ N $ 行出力せよ。$ i $ 行目 ($ 1\ <\ =\ i\ <\ =\ N $) には、$ i $ 番目に紹介されるレストランの番号を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
6
khabarovsk 20
moscow 10
kazan 50
kazan 35
moscow 60
khabarovsk 40
```

### 输出 #1

```
3
4
6
1
5
2
```

## 输入输出样例 #2

### 输入 #2

```
10
yakutsk 10
yakutsk 20
yakutsk 30
yakutsk 40
yakutsk 50
yakutsk 60
yakutsk 70
yakutsk 80
yakutsk 90
yakutsk 100
```

### 输出 #2

```
10
9
8
7
6
5
4
3
2
1
```

## 说明/提示

### 制約

- $ 1\ <\ =\ N\ <\ =\ 100 $
- $ S $ は英小文字のみからなる長さ $ 1 $ 以上 $ 10 $ 以下の文字列
- $ 0\ <\ =\ P_i\ <\ =\ 100 $
- $ P_i $ は整数
- $ P_i\ ≠\ P_j $ $ (1\ <\ =\ i\ <\ j\ <\ =\ N) $

### Sample Explanation 1

$ 3 $ 種類の市名は辞書順で `kazan` $ < $ `khabarovsk` $ < $ `moscow` です。 それぞれの市について、点数が高いレストランから順に紹介されていきます。よって、レストランは $ 3,4,6,1,5,2 $ の順に紹介されていきます。