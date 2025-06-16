# AT_abc184_a [ABC184A] Determinant

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc184/tasks/abc184_a

$ 2\ \times\ 2 $ 行列 $ A\ =\ \begin{bmatrix}\ a\ &amp;\ b\ \\ c\ &amp;\ d\ \end{bmatrix} $ が与えられます。  
 $ A $ の行列式は $ ad-bc $ で求められます。  
 $ A $ の行列式を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ a $ $ b $ $ c $ $ d $

## 输出格式

答えを整数で出力せよ。

## 输入输出样例 #1

### 输入 #1

```
1 2
3 4
```

### 输出 #1

```
-2
```

## 输入输出样例 #2

### 输入 #2

```
0 -1
1 0
```

### 输出 #2

```
1
```

## 输入输出样例 #3

### 输入 #3

```
100 100
100 100
```

### 输出 #3

```
0
```

## 说明/提示

### 制約

- 入力は全て整数
- $ -100\ \le\ a,\ b,\ c,\ d\ \le\ 100 $

### Sample Explanation 1

$ \begin{bmatrix}\ 1\ &amp;\ 2\ \\ 3\ &amp;\ 4\ \end{bmatrix} $ の行列式は $ 1\ \times\ 4\ -\ 2\ \times\ 3\ =\ -2 $ です。