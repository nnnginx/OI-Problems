# AT_arc090_d [ARC090F] Number of Digits

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc090/tasks/arc090_d

正の整数 $ n $ に対し、$ f(n) $ を $ n $ の $ 10 $ 進法での桁数と定めます。

整数 $ S $ が与えられます。 正の整数の組 $ (l,\ r) $ ($ l\ \leq\ r $) であって、$ f(l)\ +\ f(l\ +\ 1)\ +\ ...\ +\ f(r)\ =\ S $ を満たすものの個数を $ 10^9\ +\ 7 $ で割ったあまりを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
2
```

### 输出 #2

```
98
```

## 输入输出样例 #3

### 输入 #3

```
123
```

### 输出 #3

```
460191684
```

## 输入输出样例 #4

### 输入 #4

```
36018
```

### 输出 #4

```
966522825
```

## 输入输出样例 #5

### 输入 #5

```
1000
```

### 输出 #5

```
184984484
```

## 说明/提示

### 制約

- $ 1\ \leq\ S\ \leq\ 10^8 $

### Sample Explanation 1

条件を満たす $ (l,\ r) $ の組は $ (1,\ 1) $, $ (2,\ 2) $, $ ... $, $ (9,\ 9) $ の $ 9 $ 個あります。

### Sample Explanation 2

条件を満たす $ (l,\ r) $ の組は $ (1,\ 2) $ や $ (33,\ 33) $ など $ 98 $ 個あります。