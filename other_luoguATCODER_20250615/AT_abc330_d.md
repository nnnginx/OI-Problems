# AT_abc330_d [ABC330D] Counting Ls

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc330/tasks/abc330_d

$ N\ \times\ N $ のマス目が与えられます。このうち上から $ i $ 行目、左から $ j $ 列目のマスを $ (i,j) $ と書きます。  
 各マスの状態を表す $ N $ 個の長さ $ N $ の文字列 $ S_1,S_2,\dots,S_N $ が以下の形式で与えられます。

- $ S_i $ の $ j $ 文字目が `o` であるとき、 $ (i,j) $ には `o` が書かれている。
- $ S_i $ の $ j $ 文字目が `x` であるとき、 $ (i,j) $ には `x` が書かれている。
 
以下の条件を全て満たすマスの三つ組の個数を求めてください。

- 組に含まれる $ 3 $ マスは相異なる。
- $ 3 $ マス全てに `o` が書かれている。
- マスのうち、丁度 $ 2 $ つが同じ行にある。
- マスのうち、丁度 $ 2 $ つが同じ列にある。
 
但し、ふたつの三つ組は、丁度一方に含まれるマスが存在する場合のみ区別します。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S_1 $ $ S_2 $ $ \vdots $ $ S_N $

## 输出格式

答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3
ooo
oxx
xxo
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
4
oxxx
xoxx
xxox
xxxo
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
15
xooxxooooxxxoox
oxxoxoxxxoxoxxo
oxxoxoxxxoxoxxx
ooooxooooxxoxxx
oxxoxoxxxoxoxxx
oxxoxoxxxoxoxxo
oxxoxooooxxxoox
xxxxxxxxxxxxxxx
xooxxxooxxxooox
oxxoxoxxoxoxxxo
xxxoxxxxoxoxxoo
xooxxxooxxoxoxo
xxxoxxxxoxooxxo
oxxoxoxxoxoxxxo
xooxxxooxxxooox
```

### 输出 #3

```
2960
```

## 说明/提示

### 制約

- $ N $ は $ 2 $ 以上 $ 2000 $ 以下の整数
- $ S_i $ は長さ $ N $ の `o` と `x` からなる文字列
 
### Sample Explanation 1

以下の $ 4 $ つの三つ組が条件を満たします。 - $ (1,1),(1,2),(2,1) $ - $ (1,1),(1,3),(2,1) $ - $ (1,1),(1,3),(3,3) $ - $ (1,2),(1,3),(3,3) $