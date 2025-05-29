## 题目描述
The Fibonacci sequence is a sequence of integers, called Fibonacci numbers, defined as follows:

$Fib_{0}=0,Fib_{1}=1,Fib_{n}=Fib_{n-2}+Fib_{n-1}\ for\ n>1$

Its initial elements are: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, ...

Byteasar investigates representations of numbers as sums or differences of Fibonacci numbers. Currently he is wondering what is the minimum representation, i.e., one with the minimum number of (not necessarily different) Fibonacci numbers, for a given positive integer $k$ . For example, the numbers 10, 19, 17, and 1070 can be minimally represented using, respectively, 2, 2, 3, and 4 Fibonacci numbers as follows:

$10=5+5$

$19=21-2$

$17=13+5-1$

$1070=987+89-5-1$

Help Byteasar! Write a program that, for a given positive integer $k$ determines the minimum number of Fibonacci numbers required to represent $k$ as their sum or difference.

## 输入格式
In the first line of the standard input a single positive integer $p$ is given ($1\le p\le 10$) that denotes the number of queries. The following $p$ lines hold a single positive integer $k$ each ($1\le k\le 1\times 10^{17}$).


## 输出格式
For each query your program should print on the standard output the minimum number of Fibonacci numbers needed to represent the number $k$ as their sum or difference.


## 题目大意
### 题目描述

**译自 POI 2012 Stage 2. Day 2「[Rozkład Fibonacciego](https://szkopul.edu.pl/problemset/problem/w1QbhPufazp-sH6X-u4pTnNu/site/?key=statement)」**

给定正整数 $k$，求用斐波那契数的和或差表示 $k$ 所需要的斐波那契数数量最小值，例如：
- $10=5+5$
- $19=21-2$
- $17=13+5-1$
- $1070=987+89-5-1$

### 输入格式

第一行一个整数 $p (1 \le p \le 10)$ 表示询问的数量。

接下来 $p$ 行每行一个整数 $k (1 \le k \le 4 \cdot 10^{17})$。

### 输出格式

对每个询问输出一个整数，表示最少需要的斐波那契数数量。

翻译来自于 [LibreOJ](https://loj.ac/p/2697)。

```input1
1
1070
```

```output1
4
```

