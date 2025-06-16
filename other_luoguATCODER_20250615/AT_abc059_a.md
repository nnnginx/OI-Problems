# AT_abc059_a [ABC059A] Three-letter acronym

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc059/tasks/abc059_a

英小文字からなる $ 3 $ つの単語 $ s_1 $, $ s_2 $, $ s_3 $ が空白区切りで与えられるので、単語の先頭の文字をつなげ、大文字にした略語を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ s_1 $ $ s_2 $ $ s_3 $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
atcoder beginner contest
```

### 输出 #1

```
ABC
```

## 输入输出样例 #2

### 输入 #2

```
resident register number
```

### 输出 #2

```
RRN
```

## 输入输出样例 #3

### 输入 #3

```
k nearest neighbor
```

### 输出 #3

```
KNN
```

## 输入输出样例 #4

### 输入 #4

```
async layered coding
```

### 输出 #4

```
ALC
```

## 说明/提示

### 制約

- $ s_1 $, $ s_2 $, $ s_3 $ は英小文字からなる。
- $ 1\ ≦|s_i|≦\ 10\ (1≦i≦3) $

### Sample Explanation 1

`atcoder` `beginner` `contest` の先頭の文字はそれぞれ`a` `b` `c`なので、`ABC`が答えになります。