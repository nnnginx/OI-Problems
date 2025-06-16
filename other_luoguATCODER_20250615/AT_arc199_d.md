# AT_arc199_d [ARC199D] Limestone

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc199/tasks/arc199_d

正整数 $ H,W $ が与えられます．

$ H $ 行 $ W $ 列の行列 $ A=(A_{i,j})\ (1\leq\ i\leq\ H,1\leq\ j\leq\ W) $ があり，はじめ全ての要素は $ 0 $ です．

この行列に対して，以下の $ 2 $ 種類の操作を好きな順番で何度でも行うことができます．

- 整数 $ r,c\ (1\leq\ r\leq\ H,1\leq\ c\leq\ W) $ を選ぶ．$ A_{r,1},A_{r,2},\ldots,A_{r,c} $ を全て $ 1 $ にする．
- 整数 $ r,c\ (1\leq\ r\leq\ H,1\leq\ c\leq\ W) $ を選ぶ．$ A_{1,c},A_{2,c},\ldots,A_{r,c} $ を全て $ 1 $ にする．

上記の操作を繰り返して得られる行列全てに対する $ \displaystyle\ \sum_{i=1}^H\sum_{j=1}^W\ A_{i,j} $ の総和を $ 998244353 $ で割った余りを求めてください．

## 输入格式

入力は以下の形式で標準入力から与えられる．

> $ H $ $ W $

## 输出格式

操作を繰り返して得られる行列全てに対する $ \displaystyle\ \sum_{i=1}^H\sum_{j=1}^W\ A_{i,j} $ の総和を $ 998244353 $ で割った余りを出力せよ．

## 输入输出样例 #1

### 输入 #1

```
2 2
```

### 输出 #1

```
29
```

## 输入输出样例 #2

### 输入 #2

```
1 10
```

### 输出 #2

```
5120
```

## 输入输出样例 #3

### 输入 #3

```
123 456
```

### 输出 #3

```
428623282
```

## 说明/提示

### 制約

- $ 1\leq\ H,W $
- $ HW\leq\ 2\times\ 10^5 $
- 入力は全て整数

### Sample Explanation 1

操作を繰り返して得られる行列は以下の $ 14 $ 通りあります． $ \begin{pmatrix}0&amp;0\ \\ 0&amp;0\end{pmatrix}\ 
\ \begin{pmatrix}1&amp;0\ \\ 0&amp;0\end{pmatrix}\ 
\ \begin{pmatrix}0&amp;1\ \\ 0&amp;0\end{pmatrix}\ 
\ \begin{pmatrix}1&amp;1\ \\ 0&amp;0\end{pmatrix}\ 
\ \begin{pmatrix}0&amp;0\ \\ 1&amp;0\end{pmatrix}\ 
\ \begin{pmatrix}1&amp;0\ \\ 1&amp;0\end{pmatrix}\ 
\ \begin{pmatrix}0&amp;1\ \\ 1&amp;0\end{pmatrix}\ 
\ \begin{pmatrix}1&amp;1\ \\ 1&amp;0\end{pmatrix}\ 
\ \begin{pmatrix}0&amp;1\ \\ 0&amp;1\end{pmatrix}\ 
\ \begin{pmatrix}1&amp;1\ \\ 0&amp;1\end{pmatrix}\ 
\ \begin{pmatrix}0&amp;0\ \\ 1&amp;1\end{pmatrix}\ 
\ \begin{pmatrix}1&amp;0\ \\ 1&amp;1\end{pmatrix}\ 
\ \begin{pmatrix}0&amp;1\ \\ 1&amp;1\end{pmatrix}\ 
\ \begin{pmatrix}1&amp;1\ \\ 1&amp;1\end{pmatrix} $ 答えは $ 0+1+1+2+1+2+2+3+2+3+2+3+3+4=29 $ です． $ \begin{pmatrix}0&amp;0\ \\ 0&amp;1\end{pmatrix} $ や $ \begin{pmatrix}1&amp;0\ \\ 0&amp;1\end{pmatrix} $ はどのように操作しても得ることができません．