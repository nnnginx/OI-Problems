# AT_arc091_a [ABC090C] Flip,Flip, and Flip......

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc090/tasks/arc091_a

縦横に無限に広がるマス目があり、そのうちの連続する $ N $ 行 $ M $ 列の領域のすべてのマスに表裏の区別できるカードが置かれています。 最初はすべてのカードが表を向いています。

以下の操作を、カードが置かれている全てのマスについて $ 1 $ 度ずつ行います。

- そのマスと辺または点で接する $ 8 $ つのマスと、そのマスの合計 $ 9 $ マスについて、カードが存在するなら裏返す。

すべての操作を行った後の各カードの状態は操作を行う順番に依らないことが証明できます。 すべての操作を行った後、裏を向いているカードの枚数を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $

## 输出格式

すべての操作を行った後、裏を向いているカードの枚数を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 2
```

### 输出 #1

```
0
```

## 输入输出样例 #2

### 输入 #2

```
1 7
```

### 输出 #2

```
5
```

## 输入输出样例 #3

### 输入 #3

```
314 1592
```

### 输出 #3

```
496080
```

## 说明/提示

### 制約

- $ 1\ \leq\ N,M\ \leq\ 10^9 $
- 入力は全て整数である

### Sample Explanation 1

$ 4 $ 回の操作のうちのどの操作でも、すべてのカードを裏返します。よって、すべての操作を行った後は、すべてのカードが表を向いています。

### Sample Explanation 2

すべての操作を行った後は、両端以外のカードが裏を向いています。