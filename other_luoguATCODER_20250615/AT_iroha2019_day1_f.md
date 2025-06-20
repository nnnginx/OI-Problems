# AT_iroha2019_day1_f Head of The Dragon

## 题目描述

给定整数 $ N $，$ K $ 判断是否能构成满足 $a_1\ ×\ a_2\ ×\ ....\ ×\ a_K \ = N $ 的数列 $ a $，如果能构成，请在数列中按字典顺序构成一个最小的数列。除此之外，要求数列是由 **$2$ 个以上的正整数组成。**

## 输入格式

一行，正整数 $N$ 和 $K$。

> $N$ $K$

## 输出格式

如果不存在满足条件的数列，输出 `-1`；如果存在，就输出这 $K$ 个整数。

## 输入输出样例 #1

### 输入 #1

```
30 3
```

### 输出 #1

```
2 3 5
```

## 输入输出样例 #2

### 输入 #2

```
30 4
```

### 输出 #2

```
-1
```

## 输入输出样例 #3

### 输入 #3

```
123456 7
```

### 输出 #3

```
2 2 2 2 2 2 1929
```

## 说明/提示

- $ 1\ \leq\ N\ \leq\ 10^9 $
- $ 1\ \leq\ K\ \leq\ 10^9 $

样例解释 $1$：

$ 2\ × 3\ × 5\ = 30 $，所以这个数列满足条件。满足条件的还有 `3 2 5` 和 `5 2 3` 等数列也可以，但是字典顺序中最小的是 `2 3 5`，所以它是最后输出的答案。

样例解释 $2$：

怎么样都不能构成数列。