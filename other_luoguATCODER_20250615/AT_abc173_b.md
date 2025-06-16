# AT_abc173_b [ABC173B] Judge Status Summary

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc173/tasks/abc173_b

高橋君は、プログラミングコンテスト AXC002 に参加しており、問題 A にコードを提出しました。

この問題には $ N $ 個のテストケースがあります。

各テストケース $ i $ ($ 1\leq\ i\ \leq\ N $) について、ジャッジ結果を表す文字列 $ S_i $ が与えられるので、ジャッジ結果が `AC`, `WA`, `TLE`, `RE` であったものの個数をそれぞれ求めてください。

出力形式は、出力欄を参照してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ \vdots $ $ S_N $

## 输出格式

`AC`, `WA`, `TLE`, `RE` のテストケースの個数をそれぞれ $ C_0 $, $ C_1 $, $ C_2 $, $ C_3 $ としたとき、以下の形式で出力せよ。

> AC x $ C_0 $ WA x $ C_1 $ TLE x $ C_2 $ RE x $ C_3 $

## 输入输出样例 #1

### 输入 #1

```
6
AC
TLE
AC
AC
WA
TLE
```

### 输出 #1

```
AC x 3
WA x 1
TLE x 2
RE x 0
```

## 输入输出样例 #2

### 输入 #2

```
10
AC
AC
AC
AC
AC
AC
AC
AC
AC
AC
```

### 输出 #2

```
AC x 10
WA x 0
TLE x 0
RE x 0
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ S_i $ は `AC`, `WA`, `TLE`, `RE` のいずれか

### Sample Explanation 1

ジャッジ結果が `AC` であったケースが $ 3 $ 個、`WA` であったケースが $ 1 $ 個、`TLE` であったケースが $ 2 $ 個、`RE` であったケースが $ 0 $ 個でした。