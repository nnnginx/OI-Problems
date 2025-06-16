# AT_abc310_e [ABC310E] NAND repeatedly

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc310/tasks/abc310_e

`0` と `1` からなる長さ $ N $ の文字列 $ S $ が与えられます。 $ S $ は長さ $ N $ の数列 $ A=(A\ _\ 1,A\ _\ 2,\ldots,A\ _\ N) $ の情報を表しており、$ S $ の $ i $ 文字目 $ (1\leq\ i\leq\ N) $ が `0` のとき $ A\ _\ i=0 $ 、`1` のとき $ A\ _\ i=1 $です。

\\\[\\sum \_ {1\\leq i\\leq j\\leq N}(\\cdots((A \_ i\\barwedge A \_ {i+1})\\barwedge A \_ {i+2})\\barwedge\\cdots\\barwedge A \_ j)\\\]

を求めてください。

より厳密には、次のように定められる $ f(i,j)\ (1\leq\ i\leq\ j\leq\ N) $ に対して $ \displaystyle\sum\ _\ {i=1}\ ^\ {N}\sum\ _\ {j=i}\ ^\ Nf(i,j) $ を求めてください。

\\\[f(i,j)=\\left\\{\\begin{matrix} A \_ i&amp;(i=j)\\\\ f(i,j-1)\\barwedge A \_ j\\quad&amp;(i\\lt j) \\end{matrix}\\right.\\\]

ただし、否定論理積 $ \barwedge $ は次を満たす二項演算子です。

\\\[0\\barwedge0=1,0\\barwedge1=1,1\\barwedge0=1,1\\barwedge1=0\\\]

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ S $

## 输出格式

答えを $ 1 $ 行で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5
00110
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
30
101010000100101011010011000010
```

### 输出 #2

```
326
```

## 说明/提示

### 制約

- $ 1\leq\ N\leq10^6 $
- $ S $ は `0` と `1` からなる長さ $ N $ の文字列
- 入力はすべて整数
 
### Sample Explanation 1

$ 1\leq\ i\leq\ j\leq\ N $ を満たすすべての組 $ (i,j) $ に対して、$ f(i,j) $ の値は以下のようになります。 - $ f(1,1)=0=0 $ - $ f(1,2)=0\barwedge0=1 $ - $ f(1,3)=(0\barwedge0)\barwedge1=0 $ - $ f(1,4)=((0\barwedge0)\barwedge1)\barwedge1=1 $ - $ f(1,5)=(((0\barwedge0)\barwedge1)\barwedge1)\barwedge0=1 $ - $ f(2,2)=0=0 $ - $ f(2,3)=0\barwedge1=1 $ - $ f(2,4)=(0\barwedge1)\barwedge1=0 $ - $ f(2,5)=((0\barwedge1)\barwedge1)\barwedge0=1 $ - $ f(3,3)=1=1 $ - $ f(3,4)=1\barwedge1=0 $ - $ f(3,5)=(1\barwedge1)\barwedge0=1 $ - $ f(4,4)=1=1 $ - $ f(4,5)=1\barwedge0=1 $ - $ f(5,5)=0=0 $ これらの総和は $ 0+1+0+1+1+0+1+0+1+1+0+1+1+1+0=9 $ なので、$ 9 $ を出力してください。 $ \barwedge $ は結合法則を満たさないことに注意してください。 例えば、$ (1\barwedge1)\barwedge0=0\barwedge0=1\neq0=1\barwedge1=1\barwedge(1\barwedge0) $ です。