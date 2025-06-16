# AT_indeednow_2015_quala_2 Indeedなう！

## 题目描述

[problemUrl]: https://atcoder.jp/contests/indeednow-quala/tasks/indeednow_2015_quala_2

あなたには、$ N $ 個の文字列 $ {S_1,S_2,...,S_N} $が与えられます。 それぞれの $ i\ (1≦i≦N) $ について、$ S_i $ が `indeednow` のアナグラムになっているかどうかを判定しなさい。

文字列 $ A $ と $ B $ について、$ A $ に含まれる文字を任意の順番で並び替えて $ B $ にできるとき、$ A $ を $ B $ のアナグラムと呼びます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ : $ S_N $

- $ 1 $ 行目には、与えられる文字列の数 $ N\ (1≦N≦100) $ が与えられる。
- $ 2 $ 行目から $ N $ 行には、それぞれの文字列が与えられる。そのうち $ i\ (1≦i≦N) $ 行目には、$ S_i $ が与えられる。$ S_i $ の長さは $ 1 $ 以上 $ 100 $ 以下であり、半角小文字アルファベット `a`-`z` のみからなる。

## 输出格式

$ 1 $ 行目から $ N $ 行には、それぞれの文字列に対する判定結果を出力せよ。そのうち $ i\ (1≦i≦N) $ 行目には $ S_i $ が `indeednow` のアナグラムになっているならば `YES` を、そうでないならば `NO` を出力せよ。末尾の改行を忘れないこと。

## 输入输出样例 #1

### 输入 #1

```
10
nowindeed
indeedwow
windoneed
indeednow
wondeedni
a
indonow
ddeennoiw
indeednoww
indeow
```

### 输出 #1

```
YES
NO
YES
YES
YES
NO
NO
YES
NO
NO
```

## 说明/提示

### Sample Explanation 1

たとえば `nowindeed` や `windoneed` に含まれる文字を並び替えると `indeednow` にすることができます。 したがって `nowindeed` や `windoneed` は `indeednow` のアナグラムです。 一方、 `indeedwow` や `a` は、並び替えても `indeednow` にすることはできないため、`indeednow` のアナグラムではありません。