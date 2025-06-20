# AT_code_festival_2017_qualb_d 101 to 010

## 题目描述

[problemUrl]: https://atcoder.jp/contests/code-festival-2017-qualb/tasks/code_festival_2017_qualb_d

$ N $ 個のセルが一列に並んでいます。 何個かのセルはトークンを含んでいるかもしれません。 あなたは、 `0` と `1` からなる文字列 $ s $ が与えられます。 $ s $ の $ i $ 文字目が `1` のとき、(左から) $ i $ 番目のセルはトークンを一個含んでいます。 そうでないとき、トークンを含んでいません。

すぬけ君は、以下の操作をできる限り行いたいです。 各操作では、三個の連続するセルを選びます。 セルを左から $ X,\ Y,\ Z $ とします。 操作を行うためには、 $ X $ と $ Z $ の両方がトークンを含み、 $ Y $ はトークンを含んでいてはなりません。 次に、すぬけ君はこれらの二個のトークンを取り除き、新しいトークンを $ Y $ に一個置きます。

最適な操作の方法をしたとき、すぬけ君は何回操作を行えますか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ s $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
7
1010101
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
50
10101000010011011110001001111110000101010111100110
```

### 输出 #2

```
10
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 500,000 $
- $ |s|\ =\ N $
- $ s $ の各文字は `0` または `1` である。

### Sample Explanation 1

例えば、以下の方法で操作を二回行うことができます: - 最後の三個のセルに対し操作を行う。 トークンを表す文字列は `1010010` となる。 - 最初の三個のセルに対し操作を行う。 トークンを表す文字列は `0100010` となる。 操作の順番が重要であることに注意してください。 たとえば、最初に中央の三個のセルを選ぶと、それ以上操作を行えなくなります。