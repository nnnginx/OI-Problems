# AT_abc233_b [ABC233B] A Reverse

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc233/tasks/abc233_b

整数 $ L,R $ と、英小文字のみからなる文字列 $ S $ が与えられます。  
 $ S $ の $ L $ 文字目から $ R $ 文字目までの部分を反転した(すなわち、 $ L $ 文字目から $ R $ 文字目までの文字の並びを逆にした)文字列を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ L $ $ R $ $ S $

## 输出格式

問題文の指示通り出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 7
abcdefgh
```

### 输出 #1

```
abgfedch
```

## 输入输出样例 #2

### 输入 #2

```
1 7
reviver
```

### 输出 #2

```
reviver
```

## 输入输出样例 #3

### 输入 #3

```
4 13
merrychristmas
```

### 输出 #3

```
meramtsirhcyrs
```

## 说明/提示

### 制約

- $ S $ は英小文字のみからなる。
- $ 1\ \le\ |S|\ \le\ 10^5 $ ($ |S| $ は $ S $ の長さ)
- $ L,R $ は整数
- $ 1\ \le\ L\ \le\ R\ \le\ |S| $

### Sample Explanation 1

`abcdefgh` の $ 3 $ 文字目から $ 7 $ 文字目までの部分を反転すると、 `abgfedch` となります。

### Sample Explanation 2

操作を行った結果が元の文字列と同一であることもあります。