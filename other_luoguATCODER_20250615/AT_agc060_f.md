# AT_agc060_f [AGC060F] Spanning Trees of Interval Graph

## 题目描述

[problemUrl]: https://atcoder.jp/contests/agc060/tasks/agc060_f

あなたはある単純無向グラフを持っています． このグラフの各頂点には整数区間が書かれており，区間 $ [i,j] $ ($ 1\ \leq\ i\ \leq\ j\ \leq\ N $) が書かれているような頂点は $ C_{i,j} $ 個あります． また，これら以外の区間が書かれた頂点はありません．

任意の $ 2 $ つの頂点について，それらに書かれた区間が共通部分を持つとき，またそのときのみ，その $ 2 $ 頂点間の間に無向辺が存在します． ここで，区間 $ [a,b] $ と区間 $ [c,d] $ が共通部分を持つとは，$ \max(a,c)\ \leq\ \min(b,d) $ であるという意味です．

このグラフの全域木の個数を $ 998244353 $ で割ったあまりを求めてください． なお，すべての頂点は互いに区別できるものとします．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ N $ $ C_{1,1} $ $ C_{1,2} $ $ \cdots $ $ C_{1,N} $ $ C_{2,2} $ $ \cdots $ $ C_{2,N} $ $ \vdots $ $ C_{N,N} $

## 输出格式

答えを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
2
1 2
1
```

### 输出 #1

```
8
```

## 输入输出样例 #2

### 输入 #2

```
3
1 1 1
1 1
1
```

### 输出 #2

```
99
```

## 输入输出样例 #3

### 输入 #3

```
4
8 3 8 10
1 5 3
1 6
4
```

### 输出 #3

```
971555314
```

## 输入输出样例 #4

### 输入 #4

```
10
2742 5611 1401 5439 5220 8571 4998 4194 7443 2492
2393 3201 9106 1649 2456 1984 7159 9679 7695
808 4600 2573 7771 5839 9504 4381 3223
5325 2564 456 5050 6963 913 9072
310 1521 9816 6205 2988 3614
4810 2979 2852 9242 6290
7551 7139 7228 699
4869 889 7597
4239 5970
865
```

### 输出 #4

```
234850531
```

## 说明/提示

### 制約

- $ 2\ \leq\ N\ \leq\ 400 $
- $ 1\ \leq\ C_{i,j}\ \leq\ 10^4 $
- 入力される数はすべて整数