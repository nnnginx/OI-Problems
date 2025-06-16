# AT_arc182_e [ARC182E] Sum of Min of Mod of Linear

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc182/tasks/arc182_e

正整数 $ N,M,K $ と非負整数 $ C $ と長さ $ N $ の整数列 $ A=(A_1,A_2,\ldots,A_N) $ が与えられます。

$ \displaystyle\ \sum_{k=0}^{K-1}\min_{1\le\ i\le\ N}\lbrace(Ck+A_i)\ \mathrm{mod}\ M\ \rbrace $ を求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ C $ $ K $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
2 5 3 3
1 3
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
5 4 3 182
0 3 2 1 2
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
5 718 651 193855
3 532 44 109 58
```

### 输出 #3

```
29484897
```

## 说明/提示

### 制約

- $ 1\le\ N\le\ 10^5 $
- $ 1\le\ M\le\ 10^9 $
- $ 0\le\ C\ <\ M $
- $ 1\le\ K\le\ 10^9 $
- $ 0\le\ A_i\ <\ M $
- 入力はすべて整数

### Sample Explanation 1

$ k=0 $ なら $ \lbrace(3k+1)\ \mathrm{mod}\ 5\ \rbrace=1 $ 、 $ \lbrace(3k+3)\ \mathrm{mod}\ 5\ \rbrace=3 $ となるので、 $ \displaystyle\ \min_{1\le\ i\le\ N}\lbrace(Ck+A_i)\ \mathrm{mod}\ M\ \rbrace=1 $ です。 $ k=1 $ なら $ \lbrace(3k+1)\ \mathrm{mod}\ 5\ \rbrace=4 $ 、 $ \lbrace(3k+3)\ \mathrm{mod}\ 5\ \rbrace=1 $ となるので、 $ \displaystyle\ \min_{1\le\ i\le\ N}\lbrace(Ck+A_i)\ \mathrm{mod}\ M\ \rbrace=1 $ です。 $ k=2 $ なら $ \lbrace(3k+1)\ \mathrm{mod}\ 5\ \rbrace=2 $ 、 $ \lbrace(3k+3)\ \mathrm{mod}\ 5\ \rbrace=4 $ となるので、 $ \displaystyle\ \min_{1\le\ i\le\ N}\lbrace(Ck+A_i)\ \mathrm{mod}\ M\ \rbrace=2 $ です。 よって、答えは $ 1+1+2=4 $ となります。したがって、 $ 4 $ を出力してください。