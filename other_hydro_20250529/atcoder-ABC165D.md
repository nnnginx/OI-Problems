## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc165/tasks/abc165_d

整数 $ A $, $ B $, $ N $ が与えられます。

$ N $ 以下の非負整数 $ x $ に対する $ floor(Ax/B)\ -\ A\ ×\ floor(x/B) $ の最大値を求めてください。

ただし、$ floor(t) $ とは、実数 $ t $ 以下の最大の整数のことを表します。

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ N $

## 输出格式
$ N $ 以下の非負整数 $ x $ に対する $ floor(Ax/B)\ -\ A\ ×\ floor(x/B) $ の最大値を整数として出力せよ。

## 题目大意
输入$3$个数$a,b,n$，在$[1,n]$范围里找一个数$x$,使得$\lfloor \frac{ax}{b} \rfloor-a*\lfloor \frac{x}{b} \rfloor$最大

```input1
5 7 4
```

```output1
2
```

```input2
11 10 9
```

```output2
9
```

## 提示
### 制約

- $ 1\ <\ =\ A\ <\ =\ 10^{6} $
- $ 1\ <\ =\ B\ <\ =\ 10^{12} $
- $ 1\ <\ =\ N\ <\ =\ 10^{12} $
- 入力は全て整数

### Sample Explanation 1

$ x=3 $ のとき、$ floor(Ax/B)-A×floor(x/B)\ =\ floor(15/7)\ -\ 5×floor(3/7)\ =\ 2 $ となり、これが最大です。

