## 题目描述
We consider the distance between positive integers in this problem, defined as follows.

A single operation consists in either multiplying a given number by a prime number1    or dividing it by a prime number (if it does divide without a remainder).

The distance between the numbers ![](http://main.edu.pl/images/OI19/odl-en-tex.1.png) and ![](http://main.edu.pl/images/OI19/odl-en-tex.2.png), denoted ![](http://main.edu.pl/images/OI19/odl-en-tex.3.png), is the minimum number of operations    it takes to transform the number ![](http://main.edu.pl/images/OI19/odl-en-tex.4.png) into the number ![](http://main.edu.pl/images/OI19/odl-en-tex.5.png).

For example, ![](http://main.edu.pl/images/OI19/odl-en-tex.6.png).

Observe that the function ![](http://main.edu.pl/images/OI19/odl-en-tex.7.png) is indeed a distance function - for any positive integers ![](http://main.edu.pl/images/OI19/odl-en-tex.8.png), ![](http://main.edu.pl/images/OI19/odl-en-tex.9.png) and ![](http://main.edu.pl/images/OI19/odl-en-tex.10.png) the following hold:

the distance between a number and itself is 0: ![](http://main.edu.pl/images/OI19/odl-en-tex.11.png),                  the distance from ![](http://main.edu.pl/images/OI19/odl-en-tex.12.png) to ![](http://main.edu.pl/images/OI19/odl-en-tex.13.png) is the same as from ![](http://main.edu.pl/images/OI19/odl-en-tex.14.png) to ![](http://main.edu.pl/images/OI19/odl-en-tex.15.png): ![](http://main.edu.pl/images/OI19/odl-en-tex.16.png), and                  the triangle inequality holds: ![](http://main.edu.pl/images/OI19/odl-en-tex.17.png).

A sequence of ![](http://main.edu.pl/images/OI19/odl-en-tex.18.png) positive integers, ![](http://main.edu.pl/images/OI19/odl-en-tex.19.png), is given.

For each number ![](http://main.edu.pl/images/OI19/odl-en-tex.20.png) we have to determine ![](http://main.edu.pl/images/OI19/odl-en-tex.21.png) such that ![](http://main.edu.pl/images/OI19/odl-en-tex.22.png) and ![](http://main.edu.pl/images/OI19/odl-en-tex.23.png) is minimal.

## 输入格式
In the first line of standard input there is a single integer ![](http://main.edu.pl/images/OI19/odl-en-tex.24.png) (![](http://main.edu.pl/images/OI19/odl-en-tex.25.png)).

In the following ![](http://main.edu.pl/images/OI19/odl-en-tex.26.png) lines the numbers ![](http://main.edu.pl/images/OI19/odl-en-tex.27.png) (![](http://main.edu.pl/images/OI19/odl-en-tex.28.png)) are given,      one per line.

In tests worth 30% of total point it additionally holds that ![](http://main.edu.pl/images/OI19/odl-en-tex.29.png).


## 输出格式
Your program should print exactly ![](http://main.edu.pl/images/OI19/odl-en-tex.30.png) lines to the standard output, a single integer in each line.

The ![](http://main.edu.pl/images/OI19/odl-en-tex.31.png)-th line should give the minimum ![](http://main.edu.pl/images/OI19/odl-en-tex.32.png) such that: ![](http://main.edu.pl/images/OI19/odl-en-tex.33.png), ![](http://main.edu.pl/images/OI19/odl-en-tex.34.png) and ![](http://main.edu.pl/images/OI19/odl-en-tex.35.png) is minimal.


## 题目大意
### 题目描述
**译自 POI 2012 Stage 1. 「[Distance](https://szkopul.edu.pl/problemset/problem/Phel_x2Ny30OUh7z1RhCtzEG/site/?key=statement)」**

定义一次「操作」为将一个正整数除以或乘以一个质数。定义函数 $d(a,b)$ 表示将 $a$ 进行若干次“操作”变成 $b$ 所需要的最小操作次数。例如，$d(69,42)=3$.

$d$ 显然是一个距离函数，满足以下性质：
* $d(a,a) = 0$
* $d(a,b) = d(b,a)$
* $d(a,b) + d(b,c) \ge d(a,c)$

给定 $n$ 个正整数 $a_1, a_2, \ldots, a_n$，对每个 $a_i (1 \le i \le n)$，求 $j$ 使得 $j \neq i$ 且 $d(a_i,a_j)$ 最小。如果有多个满足条件的 $j$，应输出最小的那个。

### 输入格式

第一行一个正整数 $n (2 \le n \le 100,000)$.

第二行 $n$ 个正整数 $a_1, a_2, \ldots, a_n (1 \le a_i \le 1\ 000\ 000)$.

### 输出格式

输出 $n$ 行，每行一个整数，表示使 $j \neq i$ 且 $d(a_i,a_j)$ 最小的 $j$.

### 数据范围

对于 $30\%$ 的数据有 $n \le 1000$.

对于所有数据有 $2 \le n \le 10^5,1 \le a_i \le 10^6$.

翻译来自于 [LibreOJ](https://loj.ac/p/2690)。

```input1
6
1
2
3
4
5
6
```

```output1
2
1
1
2
1
2
```

