# AT_abc306_a [ABC306A] Echo

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc306/tasks/abc306_a

長さ $ N $ の英小文字からなる文字列 $ S $ が与えられます。  
$ S $ の $ i $ 文字目を $ S_i $ と記します。  
$ S_1,S_1,S_2,S_2,\dots,S_N,S_N $ をこの順に連結した長さ $ 2N $ の文字列を出力してください。  
例えば、 $ S $ が `beginner` のときは `bbeeggiinnnneerr` と出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
8
beginner
```

### 输出 #1

```
bbeeggiinnnneerr
```

## 输入输出样例 #2

### 输入 #2

```
3
aaa
```

### 输出 #2

```
aaaaaa
```

## 说明/提示

### 制約

- $ N $ は $ 1\ \le\ N\ \le\ 50 $ を満たす整数
- $ S $ は長さ $ N $ の英小文字からなる文字列

### Sample Explanation 1

問題文中の例と同じです。