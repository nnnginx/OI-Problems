# AT_abc173_a [ABC173A] Payment

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc173/tasks/abc173_a

お店で $ N $ 円の商品を買います。

$ 1000 $ 円札のみを使って支払いを行う時、お釣りはいくらになりますか？

ただし、必要最小限の枚数の $ 1000 $ 円札で支払いを行うものとします。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式

お釣りの金額を整数で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1900
```

### 输出 #1

```
100
```

## 输入输出样例 #2

### 输入 #2

```
3000
```

### 输出 #2

```
0
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10000 $
- $ N $ は整数

### Sample Explanation 1

$ 1000 $ 円札 $ 2 $ 枚で支払いを行い、お釣りは $ 100 $ 円になります。

### Sample Explanation 2

ちょうど支払えます。