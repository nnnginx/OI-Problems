# AT_tenka1_2018_b Exchange

## 题目描述

[problemUrl]: https://atcoder.jp/contests/tenka1-2018-beginner/tasks/tenka1_2018_b

高橋君は最初 $ A $ 枚、青木君は最初 $ B $ 枚のクッキーを持っています。 二人は、高橋君からはじめて交互に、以下の操作を繰り返します。

- 自分が持っているクッキーの枚数が奇数なら、自分が持っているクッキーを $ 1 $ 枚食べ、偶数なら何もしない。その後、自分が持っているクッキーの半分を相手に渡す。

合計 $ K $ 回の操作を行った後の、高橋君と青木君が持っているクッキーの枚数をそれぞれ求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ K $

## 输出格式

合計 $ K $ 回の操作を行った後の、高橋君と青木君が持っているクッキーの枚数を順に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 4 2
```

### 输出 #1

```
5 3
```

## 输入输出样例 #2

### 输入 #2

```
3 3 3
```

### 输出 #2

```
1 3
```

## 输入输出样例 #3

### 输入 #3

```
314159265 358979323 84
```

### 输出 #3

```
448759046 224379523
```

## 说明/提示

### 制約

- $ 1\ \leq\ A,B\ \leq\ 10^9 $
- $ 1\ \leq\ K\ \leq\ 100 $
- $ A,B,K $ は整数である

### Sample Explanation 1

以下のように操作は進みます。 - 最初、高橋君と青木君はそれぞれ $ 5,4 $ 枚のクッキーを持っている。 - 高橋君はクッキーを $ 1 $ 枚食べ、青木君に $ 2 $ 枚のクッキーを渡す。操作後、二人はそれぞれ $ 2,6 $ 枚のクッキーを持っている。 - 青木君は高橋君に $ 3 $ 枚のクッキーを渡す。二人はそれぞれ $ 5,3 $ 枚のクッキーを持っている。