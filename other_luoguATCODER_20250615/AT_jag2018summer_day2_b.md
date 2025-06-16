# AT_jag2018summer_day2_b Coins

## 题目描述

[problemUrl]: https://atcoder.jp/contests/jag2018summer-day2/tasks/jag2018summer_day2_b

There are $ 1 $-, $ 5 $-, $ 10 $-, $ 50 $-, $ 100 $-, $ 500 $- yen coins, and you have an infinite number of coins of each type.

For a given positive integer $ x $, let $ f(x) $ be the smallest number of coins you have to use to pay exactly $ x $ yen. For example, $ f(2018)=\ 9 $ because $ 2018\ =\ 1\ +\ 1\ +\ 1\ +\ 5\ +\ 10\ +\ 500\ +\ 500\ +\ 500\ +\ 500 $.

You are given a positive integer $ N $. Count the number of positive integers $ x $ such that $ f(x)\ =\ N $.

## 输入格式

Input is given from Standard Input in the following format:

> $ N $

## 输出格式

Print the number of positive integers $ x $ such that $ f(x)\ =\ N $.

## 输入输出样例 #1

### 输入 #1

```
1
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
2
```

### 输出 #2

```
19
```

## 输入输出样例 #3

### 输入 #3

```
1000000000000000000
```

### 输出 #3

```
500
```

## 说明/提示

### Constraints

- $ 1\ \leq\ N\ \leq\ 10^{18} $

### Sample Explanation 1

The value of $ x $ is $ 1,\ 5,\ 10,\ 50,\ 100, $ or $ 500 $.

### Sample Explanation 2

The value of $ x $ is $ 2,\ 6,\ 11,\ 15,\ 20,\ 51,\ 55,\ 60,\ 101,\ 105,\ 110,\ 150,\ 200,\ 501,\ 505,\ 510,\ 550,\ 600, $ or $ 1000 $.