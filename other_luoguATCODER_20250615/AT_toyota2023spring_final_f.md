# AT_toyota2023spring_final_f Forbidden Pattern

## 题目描述

[problemUrl]: https://atcoder.jp/contests/toyota2023spring-final/tasks/toyota2023spring_final_f

`A`, `B` からなる長さ $ N $ の文字列 $ S $ が与えられます．

あなたは，以下の操作を $ 0 $ 回以上繰り返すことができます．

- $ S $ 中の連続する $ 2 $ 文字であって，`AB` で**ない**ものを選び，消す． その後，残った左右の（空かもしれない）文字列を連結し，これを新たに $ S $ とする．

操作後の $ S $ としてあり得る文字列が何通りあるかを $ 998244353 $ で割ったあまりを求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ S $

## 输出格式

答えを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
3
BBA
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
5
ABABA
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
9
BABBAAAAB
```

### 输出 #3

```
14
```

## 输入输出样例 #4

### 输入 #4

```
48
AABABBBAABAAABAAABBBAAABBBAABAABBABAABBAAAAABBBB
```

### 输出 #4

```
3073910
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 10^6 $
- $ S $ は `A`, `B` からなる長さ $ N $ の文字列である

### Sample Explanation 1

操作後の $ S $ としてありうる文字列は，`A`, `B`, `BBA` の $ 3 $ 通りです．

### Sample Explanation 2

操作後の $ S $ としてありうる文字列は，`A`, `ABA`, `ABABA` の $ 3 $ 通りです．