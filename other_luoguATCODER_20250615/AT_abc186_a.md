# AT_abc186_a [ABC186A] Brick

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc186/tasks/abc186_a

トラックが $ 1 $ 台あります。このトラックには合計で $ N $ キログラム以下の荷物を載せることができます。

このトラックに、$ 1 $ 個 $ W $ キログラムのレンガを最大でいくつ載せることができますか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ W $

## 输出格式

トラックに載せることができるレンガの個数の最大値を整数で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
10 3
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
1000 1
```

### 输出 #2

```
1000
```

## 说明/提示

### 制約

- $ 1\leq\ N,W\ \leq\ 1000 $
- $ N,W $ は整数である。

### Sample Explanation 1

レンガは $ 1 $ 個 $ 3 $ キログラムなので、$ 3 $ 個で $ 9 $ キログラム、$ 4 $ 個で $ 12 $ キログラムになります。 したがって、$ 10 $ キログラムまで載せることができるトラックには、最大 $ 3 $ 個のレンガを載せることができます。