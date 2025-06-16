# AT_abc308_e [ABC308E] MEX

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc308/tasks/abc308_e

$ 0,1,2 $ からなる長さ $ N $ の数列 $ A=(A_1,A_2,\dots,A_N) $ と、 `M`, `E`, `X` からなる長さ $ N $ の文字列 $ S=S_1S_2\dots\ S_N $ が与えられます。

$ 1\ \leq\ i\ <\ j\ <\ k\ \leq\ N $ かつ $ S_iS_jS_k= $ `MEX` を満たす全ての整数の組 $ (i,j,k) $ に対する $ \text{mex}(A_i,A_j,A_k) $ の総和を求めてください。 ここで、$ \text{mex}(A_i,A_j,A_k) $ は $ A_i,A_j,A_k $ のいずれとも一致しない最小の非負整数を意味します。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \dots $ $ A_N $ $ S $

## 输出格式

答えを整数として出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
1 1 0 2
MEEX
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
3
0 0 0
XXX
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
15
1 1 2 0 0 2 0 2 0 0 0 0 0 2 2
EXMMXXXEMEXEXMM
```

### 输出 #3

```
13
```

## 说明/提示

### 制約

- $ 3\leq\ N\ \leq\ 2\times\ 10^5 $
- $ N $ は整数
- $ A_i\ \in\ \lbrace\ 0,1,2\rbrace $
- $ S $ は `M`, `E`, `X` からなる長さ $ N $ の文字列
 
### Sample Explanation 1

$ S_iS_jS_k $ = `MEX` となる $ i,j,k\ (1\ \leq\ i\ <\ j\ <\ k\ \leq\ N) $ の組は $ (i,j,k)=(1,2,4),(1,3,4) $ の $ 2 $ つです。 $ \text{mex}(A_1,A_2,A_4)=\text{mex}(1,1,2)=0,\text{mex}(A_1,A_3,A_4)=\text{mex}(1,0,2)=3 $ より答えは $ 0+3=3 $ です。