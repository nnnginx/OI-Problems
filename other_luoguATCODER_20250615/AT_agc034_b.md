# AT_agc034_b [AGC034B] ABC

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc034/tasks/agc034_b

`A`,`B`,`C` からなる文字列 $ s $ が与えられます。

すぬけ君は $ s $ に対して次の操作をできるだけ多く行おうとしています。

- $ s $ の連続した部分文字列であって `ABC` であるようなものをひとつ選び、 `BCA` に書き換える。

操作回数の最大値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ s $

## 输出格式

操作回数の最大値を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
ABCABC
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
C
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
ABCACCBABCBCAABCB
```

### 输出 #3

```
6
```

## 说明/提示

### 制約

- $ 1\ ≦\ |s|\ ≦\ 200000 $
- $ s $ の各文字は `A`,`B`,`C` のいずれか

### Sample Explanation 1

`ABCABC` → `BCAABC` → `BCABCA` → `BCBCAA` とすることで $ 3 $ 回操作可能で、これが最大です。