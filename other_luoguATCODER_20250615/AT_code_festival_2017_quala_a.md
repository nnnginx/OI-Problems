# AT_code_festival_2017_quala_a Snuke&#39;s favorite YAKINIKU

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2017-quala/tasks/code_festival_2017_quala_a

りんごさんは、すぬけ君にプレゼントを贈ろうとしています。

すぬけ君の好物が焼肉であることを知ったりんごさんは、すぬけ君は名前が `YAKI` から始まるものを好み、そうでないものを好まないと判断しました。

りんごさんが贈ろうと思っているものの名前を表す文字列 $ S $ が与えられます。$ S $ が `YAKI` から始まるかどうか判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

$ S $ が `YAKI` から始まるなら `Yes` を、そうでないなら `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
YAKINIKU
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
TAKOYAKI
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
YAK
```

### 输出 #3

```
No
```

## 说明/提示

### 制約

- $ 1\ \leq\ |S|\ \leq\ 10 $
- $ S $ は英大文字からなる

### Sample Explanation 1

`YAKINIKU` は `YAKI` で始まります。

### Sample Explanation 2

`TAKOYAKI` は `YAKI` で始まりません。