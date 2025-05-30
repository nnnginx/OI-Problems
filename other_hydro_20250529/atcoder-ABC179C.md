## 题目描述
[problemUrl]: https://atcoder.jp/contests/abc179/tasks/abc179_c

正整数 $ N $ が与えられます。$ A\ \times\ B\ +\ C\ =\ N $ を満たす正整数の組 $ (A,B,C) $ はいくつありますか？

## 输入格式
入力は以下の形式で標準入力から与えられる。

> $ N $

## 输出格式
答えを出力せよ。

## 题目大意
### 【题目描述】

给定一个正整数 $N$，计算有多少个正整数三元组 $(A,B,C)$ 满足 $A \times B + C = N$。

### 【输入格式】

输入一行一个正整数 $N$。

### 【输出格式】

输出一行一个整数，表示满足正整数三元组 $(A,B,C)$ 的个数。

### 【样例解释】

样例 $\#1$ 中满足条件的三元组有：$(1,1,2),(1,2,1),(2,1,1)$。

### 【数据范围】

- $2 \le N \le 10^6$。
- 输入全为正整数。

翻译由 @RP_INT_MAX 提供。

```input1
3
```

```output1
3
```

```input2
100
```

```output2
473
```

```input3
1000000
```

```output3
13969985
```

## 提示
### 制約

- $ 2\ \leq\ N\ \leq\ 10^6 $
- 入力はすべて整数

### Sample Explanation 1

$ A\ \times\ B\ +\ C\ =\ 3 $ を満たす正整数の組は、$ (A,\ B,\ C)\ =\ (1,\ 1,\ 2),\ (1,\ 2,\ 1),\ (2,\ 1,\ 1) $ の $ 3 $ つあります。

