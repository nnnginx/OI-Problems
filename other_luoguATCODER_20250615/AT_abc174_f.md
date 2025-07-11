# AT_abc174_f [ABC174F] Range Set Query

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc174/tasks/abc174_f

$ N $ 個の色の付いた玉が左右一列に並んでおり、左から $ i $ 番目の玉の色は $ c_i $ です。

クエリが $ Q $ 個与えられます。$ i $ 番目のクエリでは、左から $ l_i $ 番目から $ r_i $ 番目までにある玉の色の種類数を答えてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ Q $ $ c_1 $ $ c_2 $ $ \cdots $ $ c_N $ $ l_1 $ $ r_1 $ $ l_2 $ $ r_2 $ $ : $ $ l_Q $ $ r_Q $

## 输出格式

$ Q $ 行出力せよ。$ i $ 行目には、$ i $ 番目のクエリに対する答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4 3
1 2 1 3
1 3
2 4
3 3
```

### 输出 #1

```
2
3
1
```

## 输入输出样例 #2

### 输入 #2

```
10 10
2 5 6 5 2 1 7 9 7 2
5 5
2 4
6 7
2 2
7 8
7 9
1 8
6 9
8 10
6 8
```

### 输出 #2

```
1
2
2
1
2
2
6
3
3
3
```

## 说明/提示

### 制約

- $ 1\leq\ N,Q\ \leq\ 5\ \times\ 10^5 $
- $ 1\leq\ c_i\ \leq\ N $
- $ 1\leq\ l_i\ \leq\ r_i\ \leq\ N $
- 入力はすべて整数である。

### Sample Explanation 1

\- $ 1,2,3 $ 番目の玉の色は $ 1,2,1 $ で、色 $ 1,2 $ の $ 2 $ 種類があります。 - $ 2,3,4 $ 番目の玉の色は $ 2,1,3 $ で、色 $ 1,2,3 $ の $ 3 $ 種類があります。 - $ 3 $ 番目の玉の色は $ 1 $ で、色 $ 1 $ の $ 1 $ 種類があります。