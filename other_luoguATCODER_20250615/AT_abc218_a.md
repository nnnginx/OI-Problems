# AT_abc218_a [ABC218A] Weather Forecast

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc218/tasks/abc218_a

明日からの $ 7 $ 日間の天気予報を表す文字列 $ S $ が与えられます。  
 $ i $ 日後の予報は $ S $ の $ i $ 文字目が `o` であるとき晴れ、`x` であるとき雨です。

$ N $ 日後の天気予報が晴れかどうかを教えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式

$ N $ 日後の天気予報が晴れであるとき `Yes` を、雨であるとき `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
oooxoox
```

### 输出 #1

```
No
```

## 输入输出样例 #2

### 输入 #2

```
7
ooooooo
```

### 输出 #2

```
Yes
```

## 说明/提示

### 制約

- $ N $ は $ 1 $ 以上 $ 7 $ 以下の整数
- $ S $ は長さ $ 7 $ の文字列であり、`o` と `x` のみからなる

### Sample Explanation 1

明日からの $ 7 $ 日間の天気予報は順に、晴れ、晴れ、晴れ、雨、晴れ、晴れ、雨です。 特に、今日から $ 4 $ 日後の天気予報は雨です。