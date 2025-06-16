# AT_abc162_c [ABC162C] Sum of gcd of Tuples (Easy)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc162/tasks/abc162_c

$ \displaystyle{\sum_{a=1}^{K}\sum_{b=1}^{K}\sum_{c=1}^{K}\ \gcd(a,b,c)} $ を求めてください。

ただし、$ \gcd(a,b,c) $ は $ a,b,c $ の最大公約数を表します。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ K $

## 输出格式

$ \displaystyle{\sum_{a=1}^{K}\sum_{b=1}^{K}\sum_{c=1}^{K}\ \gcd(a,b,c)} $ の値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
200
```

### 输出 #2

```
10813692
```

## 说明/提示

### 制約

- $ 1\ \leq\ K\ \leq\ 200 $
- $ K $ は整数

### Sample Explanation 1

$ \gcd(1,1,1)+\gcd(1,1,2)+\gcd(1,2,1)+\gcd(1,2,2) $ $ +\gcd(2,1,1)+\gcd(2,1,2)+\gcd(2,2,1)+\gcd(2,2,2) $ $ =1+1+1+1+1+1+1+2=9 $ となるため、答えは $ 9 $ です。