# AT_yahoo_procon2018_qual_a yahoo

## 题目描述

[problemUrl]: https://atcoder.jp/contests/yahoo-procon2018-qual/tasks/yahoo_procon2018_qual_a

yahoo 型文字列とは、`yah` のあとに同じ英小文字が $ 2 $ つ連続した文字列を指します。例えば、`yahoo`, `yahhh` などは yahoo 型文字列ですが、 `yahoy` や `snuke` はそうではありません。

$ 5 $ 文字の英小文字からなる文字列 $ S $ が与えられるので、yahoo 型文字列かどうか判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

$ S $ が yahoo 型文字列なら `YES` を、そうでないなら `NO` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
yahoo
```

### 输出 #1

```
YES
```

## 输入输出样例 #2

### 输入 #2

```
snuke
```

### 输出 #2

```
NO
```

## 输入输出样例 #3

### 输入 #3

```
yyyyy
```

### 输出 #3

```
NO
```

## 说明/提示

### 制約

- $ |S|=5 $
- $ S $ は英小文字からなる

### Sample Explanation 1

`yahoo` は yahoo 型文字列です。

### Sample Explanation 2

`snuke` は yahoo 型文字列ではありません。