# AT_wtf19_d Distinct Boxes

## 题目描述

[problemUrl]: https://atcoder.jp/contests/wtf19/tasks/wtf19_d

すぬけ君は $ R $ 個の赤いボールと $ B $ 個の青いボールを持っています。 彼は、これらのボールを $ K $ 個の箱に分けて入れます。このとき、どの箱も空でなく、またどのふたつの箱も中身が一致しないようにします。 $ K $ のとりうる最大値を求めてください。

より形式的には、箱に $ 1 $ から $ K $ までの番号を振り、箱 $ i $ が $ r_i $ 個の赤いボールと $ b_i $ 個の青いボールを含むとすると、次の条件が満たされなければなりません。

- 各 $ i $ ($ 1\ \leq\ i\ \leq\ K $) に対し、$ r_i\ >\ 0 $ または $ b_i\ >\ 0 $ である。
- 各 $ i,\ j $ ($ 1\ \leq\ i\ <\ j\ \leq\ K $) に対し、$ r_i\ \neq\ r_j $ または $ b_i\ \neq\ b_j $ である。
- $ \sum\ r_i\ =\ R $ かつ $ \sum\ b_i\ =\ B $ である (箱の外にボールが取り残されてはならない)。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ R $ $ B $

## 输出格式

$ K $ のとりうる最大値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
8 3
```

### 输出 #1

```
5
```

## 说明/提示

### 制約

- $ 1\ \leq\ R,\ B\ \leq\ 10^{9} $

### Sample Explanation 1

$ K\ =\ 5 $ を達成する方法として考えられるものをひとつ、以下の画像に示します。 !\[\](https://img.atcoder.jp/wtf19/9ea9530037df204a84029678052ab593.png)