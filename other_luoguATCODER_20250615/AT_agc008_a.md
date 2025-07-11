# AT_agc008_a [AGC008A] Simple Calculator

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc008/tasks/agc008_a

すぬけ君は電卓を持っています。 この電卓にはディスプレイと $ 2 $ 個のボタンが付いています。

最初、ディスプレイの値は整数 $ x $ です。 すぬけ君の目標は、ディスプレイの値を整数 $ y $ にすることです。 そのために、すぬけ君は次の $ 2 $ 個のボタンを好きな順番で何回か押すことができます。

- ボタン A : ディスプレイの値を $ 1 $ 増やす。
- ボタン B : ディスプレイの値の符号を反転する。

目標を達成するためにすぬけ君がボタンを押す回数の最小値を求めてください。 なお、整数 $ x $, $ y $ の値によらず、必ず目標を達成できることが示せます。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ x $ $ y $

## 输出格式

目標を達成するためにすぬけ君がボタンを押す回数の最小値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
10 20
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
10 -10
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
-10 -20
```

### 输出 #3

```
12
```

## 说明/提示

### 制約

- $ x $, $ y $ は整数である。
- $ |x|,\ |y|\ <\ =\ 10^9 $
- $ x $, $ y $ は相異なる。

### Sample Explanation 1

ボタン A を $ 10 $ 回押せばよいです。

### Sample Explanation 2

ボタン B を $ 1 $ 回押せばよいです。

### Sample Explanation 3

次の順でボタンを押せばよいです。 - ボタン B を $ 1 $ 回押す。 - ボタン A を $ 10 $ 回押す。 - ボタン B を $ 1 $ 回押す。