# AT_abc333_g [ABC333G] Nearest Fraction

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc333/tasks/abc333_g

$ 1 $ 未満の正実数 $ r $ と正整数 $ N $ が与えられます。

$ 0\leq\ p\leq\ q\leq\ N $ かつ $ \gcd(p,q)=1 $ を満たす整数の組 $ (p,q) $ のうち、$ \left\vert\ r-\dfrac pq\right\vert $ の値を最小にするものを求めてください。

ただし、そのような $ (p,q) $ が複数存在する場合、$ \dfrac pq $ の値が最も小さいものを出力してください。

## 输入格式

入力は以下の形式で標準入力から与えられる。

> $ r $ $ N $

## 输出格式

問題文の条件を満たす $ (p,q) $ について $ p $ と $ q $ をこの順に空白区切りで一行に出力せよ。

## 输入输出样例 #1

### 输入 #1

```
0.333
33
```

### 输出 #1

```
1 3
```

## 输入输出样例 #2

### 输入 #2

```
0.45
5
```

### 输出 #2

```
2 5
```

## 输入输出样例 #3

### 输入 #3

```
0.314159265358979323
10000
```

### 输出 #3

```
71 226
```

## 输入输出样例 #4

### 输入 #4

```
0.007735339533561113
7203576162
```

### 输出 #4

```
34928144 4515398949
```

## 说明/提示

### 制約

- $ 0\lt\ r\lt\ 1 $
- $ r $ は十進法で小数点以下たかだか $ 18 $ 桁の実数として与えられる。
- $ 1\leq\ N\leq\ 10^{10} $
- $ N $ は整数
 
### Sample Explanation 1

$ \left\vert0.333-\dfrac13\right\vert=\dfrac1{3000} $ です。 $ \left\vert0.333-\dfrac\ pq\right\vert\lt\dfrac1{3000} $ となる $ 0\leq\ p\leq\ q\leq33,\gcd(p,q)=1 $ は存在しないので、`1 3` を出力してください。

### Sample Explanation 2

$ \left\vert0.45-\dfrac12\right\vert=\left\vert0.45-\dfrac25\right\vert=\dfrac1{20} $ です。 $ \left\vert0.45-\dfrac\ pq\right\vert\lt\dfrac1{20} $ となる $ 0\leq\ p\leq\ q\leq5,\gcd(p,q)=1 $ は存在せず、$ \dfrac12\gt\dfrac25 $ が成り立つので、`2 5` を出力してください。

### Sample Explanation 3

$ \left\vert0.314159265358979323-\dfrac{71}{226}\right\vert=\dfrac{3014435336501}{113000000000000000000} $ です。