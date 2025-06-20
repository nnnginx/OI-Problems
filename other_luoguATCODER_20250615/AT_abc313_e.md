# AT_abc313_e [ABC313E] Duplicate

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc313/tasks/abc313_e

`1` から `9` までの数字からなる文字列 $ S $ に対して、 $ f(S) $ を次の手順によって得られる文字列 $ T $ とします。($ S_i $ は $ S $ の $ i $ 番目の文字を意味します)

- 文字列 $ T $ がある。はじめ、$ T $ は空文字列である。
- $ i=1,\ 2,\ \dots,\ |S|\ -\ 1 $ の順に次の操作を行う。 
  - $ S_{i+1} $ を整数として解釈したときの値を $ n $ とする。$ T $ の末尾に $ S_i $ を $ n $ 個追加する。

例えば $ S\ = $ `313` のとき、以下の手順によって $ f(S)\ = $ `3111` に決まります。

- はじめ $ T $ は空文字列である。
- $ i=1 $ のとき $ n\ =\ 1 $ である。$ T $ に `3` を $ 1 $ 個追加する。$ T $ は `3` になる。
- $ i=2 $ のとき $ n\ =\ 3 $ である。$ T $ に `1` を $ 3 $ 個追加する。$ T $ は `3111` になる。
- 操作を終了する。$ T $ として `3111` を得る。

`1` から `9` までの数字からなる長さ $ N $ の文字列 $ S $ が与えられます。  
あなたは「$ S $ を $ f(S) $ に置き換える」という操作を $ S $ の長さが $ 1 $ になるまで繰り返します。  
操作が終了するまでに行う操作を行う回数を $ 998244353 $ で割った余りを求めてください。ただし、操作が無限に続く場合は `-1` を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式

操作が終了するまでに行う操作を行う回数を $ 998244353 $ で割った余りを出力せよ。ただし、操作が無限に続く場合は `-1` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
313
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
9
123456789
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
2
11
```

### 输出 #3

```
1
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 10^6 $
- $ S $ は `1`, `2`, `3`, `4`, `5`, `6`, `7`, `8`, `9` からなる長さ $ N $ の文字列

### Sample Explanation 1

$ S\ = $ `313` の場合、操作を $ 4 $ 回行うと $ S $ の長さが $ 1 $ になります。 
- $ f(S)\ = $ `3111` である。$ S $ を `3111` に置き換える。 
- $ f(S)\ = $ `311` である。$ S $ を `311` に置き換える。 
- $ f(S)\ = $ `31` である。$ S $ を `31` に置き換える。 
- $ f(S)\ = $ `3` である。$ S $ を `3` に置き換える。 
- $ S $ の長さが $ 1 $ になったので操作を終了する。

### Sample Explanation 2

$ S\ = $ `123456789` の場合、操作が無限に続きます。この場合は `-1` を出力してください。