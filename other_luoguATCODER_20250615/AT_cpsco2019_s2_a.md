# AT_cpsco2019_s2_a Scholarship Repayment

## 题目描述

[problemUrl]: https://atcoder.jp/contests/cpsco2019-s2/tasks/cpsco2019_s2_a

この春から社会人になったゴジラさんは、 $ M $ 万円の奨学金を $ N $ ヶ月間に分割して返済しようとしています。

毎月の返済額は、以下のルールによって決まっています。

- $ i $ ヶ月目( $ 1\ \leq\ i\ \leq\ N-1 $ )： $ M/N $ の小数点以下を切り捨てた金額(万円)。
- $ N $ ヶ月目：未返済の金額全て。

ゴジラさんは $ N $ ヶ月目に奨学金を何万円返済しますか。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ M $ $ N $

## 输出格式

ゴジラさんが $ N $ ヶ月目に返済する金額を万円単位で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
7 3
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
100 20
```

### 输出 #2

```
5
```

## 说明/提示

### 制約

- 入力はすべて整数である。
- $ 2\ \leq\ N\ \leq\ M\ \leq\ 100 $

### Sample Explanation 1

$ 1 $ ヶ月目と $ 2 $ ヶ月目にそれぞれ $ 2 $ 万円を返済するので、$ 3 $ ヶ月目には $ 3 $ 万円を返済します。