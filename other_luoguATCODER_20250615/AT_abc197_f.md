# AT_abc197_f [ABC197F] Construct a Palindrome

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc197/tasks/abc197_f

$ N $ 頂点 $ M $ 辺の、単純とは限らない連結な無向グラフがあります。  
 辺 $ i $ は頂点 $ A_i $ と頂点 $ B_i $ を結んでおり、文字 $ C_i $ が書かれています。  
 頂点 $ 1 $ から頂点 $ N $ へのパス (同じ辺や頂点を複数回通っても構わない) を $ 1 $ つ選び、通る辺に書かれている文字を順に並べて文字列を作ります。  
 この文字列が回文になることはあるかを判定し、あるならばそのような回文の長さとして考えられる最小値を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ A_1 $ $ B_1 $ $ C_1 $ $ A_2 $ $ B_2 $ $ C_2 $ $ A_3 $ $ B_3 $ $ C_3 $ $ \hspace{25pt}\ \vdots $ $ A_M $ $ B_M $ $ C_M $

## 输出格式

作る文字列が回文になることがあるならば、そのような回文の長さの最小値を、ないならば `-1` を出力せよ。

## 输入输出样例 #1

### 输入 #1

```
8 8
1 2 a
2 3 b
1 3 c
3 4 b
4 5 a
5 6 c
6 7 b
7 8 a
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
4 5
1 1 a
1 2 a
2 3 a
3 4 b
4 4 a
```

### 输出 #2

```
5
```

## 输入输出样例 #3

### 输入 #3

```
3 4
1 1 a
1 2 a
2 3 b
3 3 b
```

### 输出 #3

```
-1
```

## 说明/提示

### 制約

- $ 2\ \le\ N\ \le\ 1000 $
- $ 1\ \le\ M\ \le\ 1000 $
- $ 1\ \le\ A_i\ \le\ N $
- $ 1\ \le\ B_i\ \le\ N $
- $ C_i $ は英小文字
- 与えられるグラフは連結である

### Sample Explanation 1

辺 $ 1,\ 2,\ 3,\ 1,\ 2,\ 4,\ 5,\ 6,\ 7,\ 8 $ の順に通ると、出来上がる文字列は `abcabbacba` となり、回文となります。 これより短い回文を作ることはできないので、答えは $ 10 $ です。

### Sample Explanation 2

辺 $ 2,\ 3,\ 4,\ 5,\ 5 $ の順に通ると `aabaa` という文字列を作ることができ、これは回文です。 同じ辺や頂点を複数回通っても構わないことに注意してください。

### Sample Explanation 3

出来上がる文字列が回文となることはありません。