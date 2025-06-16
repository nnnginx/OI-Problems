# AT_abc264_d [ABC264D] "redocta".swap(i,i+1)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc264/tasks/abc264_d

`atcoder` の並べ替えである文字列 $ S $ が与えられます。  
この文字列 $ S $ に対して以下の操作を $ 0 $ 回以上行います。

- $ S $ 中の隣接する $ 2 $ 文字を選び、入れ替える。

$ S $ を `atcoder` にするために必要な最小の操作回数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ S $

## 输出格式

答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
catredo
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
atcoder
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
redocta
```

### 输出 #3

```
21
```

## 说明/提示

### 制約

- $ S $ は `atcoder` の並べ替えである文字列

### Sample Explanation 1

`catredo` $ \rightarrow $ `\[ac\]tredo` $ \rightarrow $ `actre\[od\]` $ \rightarrow $ `actr\[oe\]d` $ \rightarrow $ `actro\[de\]` $ \rightarrow $ `act\[or\]de` $ \rightarrow $ `acto\[dr\]e` $ \rightarrow $ `a\[tc\]odre` $ \rightarrow $ `atcod\[er\]` という流れで操作を行うと、 $ 8 $ 回で $ S $ を `atcoder` にすることができ、これが達成可能な最小の操作回数です。

### Sample Explanation 2

この場合、文字列 $ S $ は元から `atcoder` です。