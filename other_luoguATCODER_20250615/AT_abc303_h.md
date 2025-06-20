# AT_abc303_h [ABC303Ex] Constrained Tree Degree

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc303/tasks/abc303_h

整数 $ N $ 及び $ 1 $ 以上 $ N-1 $ 以下の整数からなる集合 $ S=\lbrace\ S_1,S_2,\ldots,S_K\rbrace $ が与えられます。

頂点に $ 1 $ から $ N $ の番号がついた $ N $ 頂点の木 $ T $ のうち、以下の条件を満たすものの個数を $ 998244353 $ で割った余りを答えてください。

- 任意の $ i\ (1\leq\ i\ \leq\ N) $ について、$ T $ の頂点 $ i $ の次数を $ d_i $ としたとき、 $ d_i\in\ S $

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ S_1 $ $ \ldots $ $ S_K $

## 输出格式

条件を満たす木 $ T $ の個数を $ 998244353 $ で割った余りを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 2
1 3
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
10 5
1 2 3 5 6
```

### 输出 #2

```
68521950
```

## 输入输出样例 #3

### 输入 #3

```
100 5
1 2 3 14 15
```

### 输出 #3

```
888770956
```

## 说明/提示

### 制約

- $ 2\leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\leq\ K\ \leq\ N-1 $
- $ 1\leq\ S_1\ <\ S_2\ <\ \ldots\ <\ S_K\ \leq\ N-1 $
- 入力は全て整数

### Sample Explanation 1

ある $ 1 $ つの頂点の次数が $ 3 $ であり、ほかの頂点の次数が $ 1 $ であるような木が条件を満たします。よって答えは $ 4 $ 個です。

### Sample Explanation 3

個数を $ 998244353 $ で割った余りを出力してください。