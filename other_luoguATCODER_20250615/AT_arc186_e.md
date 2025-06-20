# AT_arc186_e [ARC186E] Missing Subsequence

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc186/tasks/arc186_e

$ 1,\dots,K $ からなる長さ $ M $ の整数列 $ (X_1,\dots,X_M) $ が与えられます。

$ 1,\dots,K $ からなる長さ $ N $ の整数列 $ (A_1,\dots,A_N) $ のうち、以下の条件を満たすものの数を $ 998244353 $ で割ったあまりを求めてください。

- $ 1,\dots,K $ からなる長さ $ M $ の整数列のうち、$ (A_1,\dots,A_N) $ の（連続とは限らない）部分列として取れないものは $ (X_1,\dots,X_M) $ のみ

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ N $ $ M $ $ K $ $ X_1 $ $ X_2 $ $ \dots $ $ X_M $

## 输出格式

条件を満たす数列の数を $ 998244353 $ で割ったあまりを出力せよ。

## 输入输出样例 #1

### 输入 #1

```
5 2 3
1 1
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
400 3 9
1 8 6
```

### 输出 #2

```
417833302
```

## 输入输出样例 #3

### 输入 #3

```
29 3 10
3 3 3
```

### 输出 #3

```
495293602
```

## 输入输出样例 #4

### 输入 #4

```
29 3 10
3 3 4
```

### 输出 #4

```
0
```

## 说明/提示

### 制約

- $ 2\le\ M,K\ \le\ N\ \le\ 400 $
- $ 1\le\ X_i\ \le\ K $
- 入力はすべて整数
 
### Sample Explanation 1

以下の $ 4 $ 通りが条件を満たします。 - $ (2,\ 3,\ 1,\ 2,\ 3) $ - $ (2,\ 3,\ 1,\ 3,\ 2) $ - $ (3,\ 2,\ 1,\ 2,\ 3) $ - $ (3,\ 2,\ 1,\ 3,\ 2) $