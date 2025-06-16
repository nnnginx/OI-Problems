# AT_abc164_c [ABC164C] gacha

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc164/tasks/abc164_c

くじ引きを $ N $ 回行い、$ i $ 回目には種類が文字列 $ S_i $ で表される景品を手に入れました。

何種類の景品を手に入れましたか？

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ : $ $ S_N $

## 输出格式

何種類の景品を手に入れたか出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
apple
orange
apple
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
5
grape
grape
grape
grape
grape
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
4
aaaa
a
aaa
aa
```

### 输出 #3

```
4
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ S_i $ は英小文字のみからなり、長さは $ 1 $ 以上 $ 10 $ 以下

### Sample Explanation 1

`apple` と `orange` の $ 2 $ 種類の景品を手に入れました。