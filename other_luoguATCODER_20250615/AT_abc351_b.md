# AT_abc351_b [ABC351B] Spot the Difference

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc351/tasks/abc351_b

縦 $ N $ マス、横 $ N $ マスのグリッドが $ 2 $ 個与えられます。それぞれグリッド $ A $, グリッド $ B $ と呼びます。  
 グリッドの各マスには英小文字が書かれています。  
 グリッド $ A $ の上から $ i $ 行目、左から $ j $ 列目に書かれている文字は $ A_{i,\ j} $ です。  
 グリッド $ B $ の上から $ i $ 行目、左から $ j $ 列目に書かれている文字は $ B_{i,\ j} $ です。

2 つのグリッドは $ 1 $ ヵ所だけ書かれている文字が異なります。すなわち、$ A_{i,\ j}\ \neq\ B_{i,\ j} $ である $ N $ 以下の正整数の組 $ (i,\ j) $ はちょうど $ 1 $ 個存在します。この $ (i,\ j) $ を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_{1,1}A_{1,2}\dots\ A_{1,N} $ $ A_{2,1}A_{2,2}\dots\ A_{2,N} $ $ \vdots $ $ A_{N,1}A_{N,2}\dots\ A_{N,N} $ $ B_{1,1}B_{1,2}\dots\ B_{1,N} $ $ B_{2,1}B_{2,2}\dots\ B_{2,N} $ $ \vdots $ $ B_{N,1}B_{N,2}\dots\ B_{N,N} $

## 输出格式

$ A_{i,\ j}\ \neq\ B_{i,\ j} $ である $ N $ 以下の正整数の組を $ (i,\ j) $ とする。この時、$ (i,\ j) $ を以下の形式で出力せよ。

> $ i $ $ j $

## 输入输出样例 #1

### 输入 #1

```
3
abc
def
ghi
abc
bef
ghi
```

### 输出 #1

```
2 1
```

## 输入输出样例 #2

### 输入 #2

```
1
f
q
```

### 输出 #2

```
1 1
```

## 输入输出样例 #3

### 输入 #3

```
10
eixfumagit
vtophbepfe
pxbfgsqcug
ugpugtsxzq
bvfhxyehfk
uqyfwtmglr
jaitenfqiq
acwvufpfvv
jhaddglpva
aacxsyqvoj
eixfumagit
vtophbepfe
pxbfgsqcug
ugpugtsxzq
bvfhxyehok
uqyfwtmglr
jaitenfqiq
acwvufpfvv
jhaddglpva
aacxsyqvoj
```

### 输出 #3

```
5 9
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 100 $
- $ A_{i,\ j},\ B_{i,\ j} $ は全て英小文字
- $ A_{i,\ j}\ \neq\ B_{i,\ j} $ である $ (i,\ j) $ がちょうど $ 1 $ 個存在する
 
### Sample Explanation 1

$ A_{2,\ 1}\ = $ `d`、$ B_{2,\ 1} $ = `b` なので $ A_{2,\ 1}\ \neq\ B_{2,\ 1} $ が成り立つため、$ (i,\ j)\ =\ (2,\ 1) $ は問題文の条件を満たします。