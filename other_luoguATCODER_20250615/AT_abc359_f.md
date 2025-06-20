# AT_abc359_f [ABC359F] Tree Degree Optimization

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc359/tasks/abc359_f

整数列 $ A=(A_1,\ldots,A_N) $ が与えられます。 $ N $ 頂点の木 $ T $ に対して、 $ f(T) $ を以下で定めます。

- $ T $ の頂点 $ i $ の次数を $ d_i $ とする。このとき、$ f(T)=\sum_{i=1}^N\ {d_i}^2\ A_i $ とする。
 
$ f(T) $ として考えられる最小値を求めてください。

なお、制約下において答えが $ 2^{63} $ 未満となることは保証されています。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ A_1 $ $ A_2 $ $ \ldots $ $ A_N $

## 输出格式

答えを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
4
3 2 5 2
```

### 输出 #1

```
24
```

## 输入输出样例 #2

### 输入 #2

```
3
4 3 2
```

### 输出 #2

```
15
```

## 输入输出样例 #3

### 输入 #3

```
7
10 5 10 2 10 13 15
```

### 输出 #3

```
128
```

## 说明/提示

### 制約

- $ 2\leq\ N\leq\ 2\times\ 10^5 $
- $ 1\leq\ A_i\ \leq\ 10^9 $
- 入力される数値は全て整数
 
### Sample Explanation 1

頂点 $ 1 $ と頂点 $ 2 $ を結ぶ辺、頂点 $ 2 $ と頂点 $ 4 $ を結ぶ辺、頂点 $ 4 $ と頂点 $ 3 $ を結ぶ辺からなるような木 $ T $ を考えます。 このとき $ f(T)\ =\ 1^2\times\ 3\ +\ 2^2\times\ 2+1^2\times\ 5\ +2^2\times\ 2\ =\ 24 $ です。これが $ f(T) $ の最小値であることが証明できます。