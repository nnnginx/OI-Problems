# AT_abc154_c [ABC154C] Distinct or Not

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc154/tasks/abc154_c

整数列 $ A_1,\ A_2,\ ...,\ A_N $ が与えられます。 この整数列のどの $ 2 $ つの要素も互いに異なるならば `YES` を、そうでないなら `NO` を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ ... $ $ A_N $

## 输出格式

整数列のどの $ 2 $ つの要素も互いに異なるならば `YES` を、そうでないなら `NO` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
2 6 1 4 5
```

### 输出 #1

```
YES
```

## 输入输出样例 #2

### 输入 #2

```
6
4 1 3 1 6 2
```

### 输出 #2

```
NO
```

## 输入输出样例 #3

### 输入 #3

```
2
10000000 10000000
```

### 输出 #3

```
NO
```

## 说明/提示

### 制約

- $ 2\ <\ =\ N\ <\ =\ 200000 $
- $ 1\ <\ =\ A_i\ <\ =\ 10^9 $
- 入力は全て整数

### Sample Explanation 1

どの $ 2 $ つの要素も互いに異なります。

### Sample Explanation 2

$ 2 $ 番目の要素と $ 4 $ 番目の要素が同じです。