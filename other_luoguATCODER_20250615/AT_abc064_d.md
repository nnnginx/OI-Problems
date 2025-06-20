# AT_abc064_d [ABC064D] Insertion

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc064/tasks/abc064_d

`(` と `)` で構成される $ N $ 文字の文字列 $ S $ が与えられる。$ S $ にいくつかの `(` または `)` を挿入することで正しい括弧列を作りたい。  
 ただし、正しい括弧列は次のように定義されている：

- `()` は正しい括弧列である。
- $ X $ が正しい括弧列であるとき、`(`、$ X $、`)` をこの順につなげたものは正しい括弧列である。
- $ X $、$ Y $ が正しい括弧列であるとき、$ X $ と $ Y $ をこの順につなげたものは正しい括弧列である。
- それ以外の括弧列は正しくない。

そのとき、作れる最も文字数が少ない正しい括弧列を求めなさい。このようなものが複数ある場合は、辞書順最小のものを求めなさい。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式

$ S $ から `(`、`)` を挿入していったときに作れる最小の長さの正しい括弧列のなかで辞書順最小の文字列を出力しなさい。

## 输入输出样例 #1

### 输入 #1

```
3
())
```

### 输出 #1

```
(())
```

## 输入输出样例 #2

### 输入 #2

```
6
)))())
```

### 输出 #2

```
(((()))())
```

## 输入输出样例 #3

### 输入 #3

```
8
))))((((
```

### 输出 #3

```
(((())))(((())))
```

## 说明/提示

### 制約

- $ S $ の長さは $ N $ である。
- $ 1\ <\ =\ N\ <\ =\ 100 $
- $ S $ は `(` と `)` のみで構成されている。