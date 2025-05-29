## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc230/tasks/abc230_e

正の整数 $ N $ が与えられます。 $ \displaystyle\sum_{i=1}^N\ \left[\ \frac{N}{i}\ \right] $ の値を求めてください。

ただし、実数 $ x $ に対して $ [x] $ で $ x $ 以下の最大の整数を表します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
答えを出力せよ。

## 题目大意
## 题目描述

求 $\large{\sum\limits_{i=1}^N ⌊\frac{N}{i}⌋}$ 的值

## 输入格式

一行一个整数 $N$ 

## 输出格式

一行一个整数，你的答案

```input1
3
```

```output1
5
```

```input2
10000000000
```

```output2
231802823220
```

## 提示
### 制約

- $ 1\ \leq\ N\ \leq\ 10^{12} $
- $ N $ は整数である。

### Sample Explanation 1

$ \left[\ \frac{3}{1}\ \right]+\left[\ \frac{3}{2}\ \right]+\left[\ \frac{3}{3}\ \right]=3+1+1=5 $ です。

### Sample Explanation 2

入力や出力が $ 32 $ bit 整数型に収まらないことがあることに注意してください。

