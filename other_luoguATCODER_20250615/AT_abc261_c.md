# AT_abc261_c [ABC261C] NewFolder(1)

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc261/tasks/abc261_c

$ 2 $ つの文字列 $ A,B $ に対して、$ A $ の末尾に $ B $ を連結した文字列を $ A+B $ と表します。

$ N $ 個の文字列 $ S_1,\ldots,S_N $ が与えられます。$ i=1,\ldots,N $ の順に、次の指示に従って加工して出力してください。

- $ S_1,\ldots,S_{i-1} $ の中に $ S_i $ と同じ文字列が存在しないならば、$ S_i $ を出力する。
- $ S_1,\ldots,S_{i-1} $ の中に $ S_i $ と同じ文字列が $ X $ 個 $ (X\ >\ 0) $ 存在するならば、$ X $ を文字列として扱って $ S_i+ $ `(` $ +X+ $ `)` を出力する。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式

問題文中の指示にしたがって、$ N $ 行出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
newfile
newfile
newfolder
newfile
newfolder
```

### 输出 #1

```
newfile
newfile(1)
newfolder
newfile(2)
newfolder(1)
```

## 输入输出样例 #2

### 输入 #2

```
11
a
a
a
a
a
a
a
a
a
a
a
```

### 输出 #2

```
a
a(1)
a(2)
a(3)
a(4)
a(5)
a(6)
a(7)
a(8)
a(9)
a(10)
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ S_i $ は英小文字のみからなる長さ $ 1 $ 以上 $ 10 $ 以下の文字列