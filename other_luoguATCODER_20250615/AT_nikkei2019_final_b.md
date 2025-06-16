# AT_nikkei2019_final_b Big Integers

## 题目描述

[problemUrl]: https://atcoder.jp/contests/nikkei2019-final/tasks/nikkei2019_final_b

長さ $ N $ の整数列 $ A $、長さ $ M $ の整数列 $ B $、整数 $ K $ が与えられます。 値 $ X,Y $ を以下のように定義します。

- $ X=\ \sum_{i=1}^N\ A_i\ \times\ K^{N-i}\ =\ A_1\ \times\ K^{N-1}\ +\ A_2\ \times\ K^{N-2}\ +\ ...\ +\ A_N\ \times\ K^0 $
- $ Y=\ \sum_{i=1}^M\ B_i\ \times\ K^{M-i}\ =\ B_1\ \times\ K^{M-1}\ +\ B_2\ \times\ K^{M-2}\ +\ ...\ +\ B_M\ \times\ K^0 $

$ X $ と $ Y $ のどちらが小さいかを求めてください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ K $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $ $ B_1 $ $ B_2 $ $ \cdots $ $ B_M $

## 输出格式

$ X\ <\ Y $ のときは `X`、$ X\ >\ Y $ のときは `Y`、$ X\ =\ Y $ のときは `Same` と出力せよ。

## 输入输出样例 #1

### 输入 #1

```
3 3 10
1 2 3
1 2 4
```

### 输出 #1

```
X
```

## 输入输出样例 #2

### 输入 #2

```
4 3 13
1 2 3 4
4 5 6
```

### 输出 #2

```
Y
```

## 输入输出样例 #3

### 输入 #3

```
4 4 2
1 1 0 1
1 1 0 1
```

### 输出 #3

```
Same
```

## 说明/提示

### 制約

- $ 1\ \leq\ N\ \leq\ 10^5 $
- $ 1\ \leq\ M\ \leq\ 10^5 $
- $ 2\ \leq\ K\ \leq\ 10^9 $
- $ 0\ \leq\ A_i\ \leq\ K-1 $
- $ 1\ \leq\ A_1 $
- $ 0\ \leq\ B_i\ \leq\ K-1 $
- $ 1\ \leq\ B_1 $
- 入力される値はすべて整数である。

### Sample Explanation 1

$ X=123,Y=124 $ であり、 $ X\ <\ Y $ であるので `X` と出力します。