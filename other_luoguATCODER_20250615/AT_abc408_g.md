# AT_abc408_g [ABC408G] A/B < p/q < C/D

## 题目描述

给你四个正整数 $A,B,C,D$，满足 $\displaystyle \frac{A}{B}<\displaystyle \frac{C}{D}$。请求出最小的正整数 $q$，满足存在一个正整数 $p$ 使得 $\displaystyle \frac{A}{B}<\displaystyle \frac{p}{q}<\displaystyle \frac{C}{D}$。

可以证明这样的 $q$ 存在。多组数据。

## 输入格式

多组数据。第一行一个整数 $T(1\le T\le 2\times 10^5)$ 表示数据组数。

对于每组数据，输入一行四个正整数 $A,B,C,D(1\le A,B,C,D\le 10^{18})$。

## 输出格式

对于每组数据，输出一行一个整数表示答案。

## 输入输出样例 #1

### 输入 #1

```
5
3 2 2 1
5 2 8 3
1 2 2 1
60 191 11 35
40 191 71 226
```

### 输出 #1

```
3
5
1
226
4
```

## 说明/提示

**样例解释**

对于第一组数据，令 $p=5,q=3$，有 $\displaystyle \frac{3}{2}<\displaystyle \frac{5}{3}<\displaystyle \frac{2}{1}$，所以 $q=3$ 是可行的。

可以证明 $q$ 没有更小的正整数解，故答案为 $3$。

By @[chenxi2009](/user/1020063)