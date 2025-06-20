# AT_abc052_a [ABC052A] Two Rectangles

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc052/tasks/abc052_a

二つの長方形があります。 一つ目の長方形は、縦の辺の長さが $ A $、横の辺の長さが $ B $ です。 二つ目の長方形は、縦の辺の長さが $ C $、横の辺の長さが $ D $ です。

この二つの長方形のうち、面積の大きい方の面積を出力してください。 なお、二つの長方形の面積が等しい時は、その面積を出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ A $ $ B $ $ C $ $ D $

## 输出格式

大きい方の長方形の面積を出力せよ。 二つの長方形の面積が等しいなら、その面積を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 5 2 7
```

### 输出 #1

```
15
```

## 输入输出样例 #2

### 输入 #2

```
100 600 200 300
```

### 输出 #2

```
60000
```

## 说明/提示

### 制約

- 入力は全て整数である
- $ 1≦A≦10^4 $
- $ 1≦B≦10^4 $
- $ 1≦C≦10^4 $
- $ 1≦D≦10^4 $

### Sample Explanation 1

一つ目の長方形の面積は $ 3×5=15 $ で、二つ目の長方形の面積は $ 2×7=14 $ です。 よって、大きい方の面積である $ 15 $ を出力します。

### Sample Explanation 2

どちらの長方形の面積も $ 60000 $ なので、$ 60000 $ を出力します。