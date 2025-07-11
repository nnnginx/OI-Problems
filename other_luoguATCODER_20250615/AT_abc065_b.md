# AT_abc065_b [ABC065B] Trained?

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc065/tasks/abc065_b

筋力をつけたい高橋君は、AtCoder 社のトレーニング設備で、トレーニングをすることにしました。

AtCoder 社のトレーニング設備には $ N $ 個のボタンがついており、ちょうど $ 1 $ 個のボタンが光っています。 ボタンには、$ 1 $ から $ N $ までの番号がついています。 ボタン $ i $ が光っているときにそのボタンを押すと、ボタン $ i $ の明かりが消え、その後ボタン $ a_i $ が光ります。$ i=a_i $ であることもあります。 光っていないボタンを押しても、何も起こりません。

最初、ボタン $ 1 $ が光っています。高橋君は、ボタン $ 2 $ が光っている状態で、トレーニングをやめたいと思っています。

そのようなことは可能かどうか判定し、もし可能なら最低で何回ボタンを押す必要があるかを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ a_1 $ $ a_2 $ : $ a_N $

## 输出格式

ボタン $ 2 $ を光らせることが不可能な場合、$ -1 $ を出力せよ。 そうでない場合、ボタン $ 2 $ を光らせるために必要なボタンを押す回数の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
3
1
2
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
4
3
4
1
2
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
5
3
3
4
2
4
```

### 输出 #3

```
3
```

## 说明/提示

### 制約

- $ 2\ ≦\ N\ ≦\ 10^5 $
- $ 1\ ≦\ a_i\ ≦\ N $

### Sample Explanation 1

ボタン $ 1,3 $ の順に押せばよいです。

### Sample Explanation 2

ボタン $ 1 $ を押すとボタン $ 3 $ 、ボタン $ 3 $ を押すとボタン $ 1 $ が光るので、ボタン $ 2 $ が光ることはありません。