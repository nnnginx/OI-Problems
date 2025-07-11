# AT_abc171_b [ABC171B] Mix Juice

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc171/tasks/abc171_b

ある店で $ N $ 種類の果物、果物 $ 1,\ \ldots,\ N $ が売られており、それぞれの価格は一個あたり $ p_1,\ \ldots,\ p_N $ 円です。

この店で $ K $ 種類の果物を一個ずつ買うとき、それらの合計価格として考えられる最小の金額を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ p_1 $ $ p_2 $ $ \ldots $ $ p_N $

## 输出格式

果物の最小の合計価格を表す整数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 3
50 100 80 120 80
```

### 输出 #1

```
210
```

## 输入输出样例 #2

### 输入 #2

```
1 1
1000
```

### 输出 #2

```
1000
```

## 说明/提示

### 制約

- $ 1\ \leq\ K\ \leq\ N\ \leq\ 1000 $
- $ 1\ \leq\ p_i\ \leq\ 1000 $
- 入力中の値はすべて整数である。

### Sample Explanation 1

この店では、果物 $ 1,\ 2,\ 3,\ 4,\ 5 $ がそれぞれ $ 50 $ 円、$ 100 $ 円、$ 80 $ 円、$ 120 $ 円、$ 80 $ 円で売られています。 これらから $ 3 $ 種類を買うときの最小合計価格は、果物 $ 1,\ 3,\ 5 $ を買うときの $ 50\ +\ 80\ +\ 80\ =\ 210 $ 円です。