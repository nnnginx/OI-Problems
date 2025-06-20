# AT_abc176_b [ABC176B] Multiple of 9

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc176/tasks/abc176_b

整数 $ N $ が $ 9 $ の倍数であることと、$ N $ を十進法で表したときの各桁の数の和が $ 9 $ の倍数であることは同値です。

$ N $ が $ 9 $ の倍数であるか判定してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式

$ N $ が $ 9 $ の倍数ならば `Yes`、そうでないなら `No` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
123456789
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
0
```

### 输出 #2

```
Yes
```

## 输入输出样例 #3

### 输入 #3

```
31415926535897932384626433832795028841971693993751058209749445923078164062862089986280
```

### 输出 #3

```
No
```

## 说明/提示

### 制約

- $ 0\ \leq\ N\ <\ 10^{200000} $
- $ N $ は整数

### Sample Explanation 1

各桁の数の和は $ 1+2+3+4+5+6+7+8+9=45 $ であり、$ 45 $ は $ 9 $ の倍数なので、$ 123456789 $ は $ 9 $ の倍数です。