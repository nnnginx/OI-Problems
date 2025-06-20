# AT_abc146_e [ABC146E] Rem of Sum is Num

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc146/tasks/abc146_e

長さ $ N $ の正整数列 $ A_1,\ A_2,\ \ldots\ ,\ A_N $ と正の整数 $ K $ が与えられます。

$ A $ の空でない連続する部分列であって、要素の和を $ K $ で割った余りが要素の数と等しくなるものの数を求めてください。ただし、$ 2 $ つの部分列が列として同じでも、取り出す位置が異なるならば区別するものとします。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ K $ $ A_1 $ $ A_2 $ $ \cdots $ $ A_N $

## 输出格式

条件をみたす部分列の個数を出力してください。

## 输入输出样例 #1

### 输入 #1

```
5 4
1 4 2 3 5
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
8 4
4 2 4 2 4 2 4 2
```

### 输出 #2

```
7
```

## 输入输出样例 #3

### 输入 #3

```
10 7
14 15 92 65 35 89 79 32 38 46
```

### 输出 #3

```
8
```

## 说明/提示

### 制約

- 入力は全て整数である。
- $ 1\ \leq\ N\ \leq\ 2\times\ 10^5 $
- $ 1\ \leq\ K\ \leq\ 10^9 $
- $ 1\ \leq\ A_i\ \leq\ 10^9 $

### Sample Explanation 1

$ (1) $, $ (4,2) $, $ (1,4,2) $, $ (5) $ の $ 4 $ つが条件をみたす部分列です。

### Sample Explanation 2

$ (4,2) $ が $ 4 $ 回、$ (2,4) $ が $ 3 $ 回数えられています。