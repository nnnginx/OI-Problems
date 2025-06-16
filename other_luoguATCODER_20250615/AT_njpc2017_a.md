# AT_njpc2017_a 入力フォーム

## 题目描述

[problemUrl]: https://atcoder.jp/contests/njpc2017/tasks/njpc2017_a

英小文字のみからなる文字列 $ S $ と 表示する最大の長さ $ L $ が入力として与えられる。

$ S $ の文字数が $ L $ より大きい場合は初めの $ L $ 文字のみを出力せよ。そうでない場合には $ S $ をそのまま出力せよ。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ L $ $ S $

## 输出格式

処理した後の文字列を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
10
hello
```

### 输出 #1

```
hello
```

## 输入输出样例 #2

### 输入 #2

```
37
narasenntannkagakugijyutudaigakuinndaigaku
```

### 输出 #2

```
narasenntannkagakugijyutudaigakuinnda
```

## 说明/提示

### ストーリー

こんにちは。NJPCにご参加いただきありがとうございます。

NJPCの正式名称は「Nara institute of science and technology &amp; Japan advanced institute of science and technology Programming Contest」というのですが、いかんせん長すぎます。

そこであなたに、長過ぎる文字列は初めの $ L $ 文字のみを表示するプログラムの作成をお願いしたいのです。

### 制約

- $ 1≦L,|S|≦10^5 $
- $ L $ は整数である
- $ S $ は英小文字のみからなる