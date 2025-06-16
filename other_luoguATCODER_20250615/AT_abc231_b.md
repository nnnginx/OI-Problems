# AT_abc231_b [ABC231B] Election

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc231/tasks/abc231_b

選挙が行われています。

$ N $ 人が投票を行い、$ i\,(1\ \leq\ i\ \leq\ N) $ 番目の人は $ S_i $ という名前の候補者に投票しました。

得票数が最大の候補者の名前を答えてください。なお、与えられる入力では得票数が最大の候補者は一意に定まります。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式

得票数が最大の候補者の名前を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
snuke
snuke
takahashi
takahashi
takahashi
```

### 输出 #1

```
takahashi
```

## 输入输出样例 #2

### 输入 #2

```
5
takahashi
takahashi
aoki
takahashi
snuke
```

### 输出 #2

```
takahashi
```

## 输入输出样例 #3

### 输入 #3

```
1
a
```

### 输出 #3

```
a
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ S_i $ は英小文字からなる長さ $ 1 $ 以上 $ 10 $ 以下の文字列
- $ N $ は整数
- 得票数が最大の候補者は一意に定まる

### Sample Explanation 1

`takahashi` は $ 3 $ 票、`snuke` は $ 2 $ 票獲得しました。よって `takahashi` を出力します。