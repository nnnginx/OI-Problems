## 题目描述
Byteasar has decided to build a house.

He has chosen a very narrow valley as its location.

Before Byteasar starts the actual construction work, he has to level the ground first.

He has two excavators at his disposal: the first one can either increase or decrease the  ground level of any connected area in the valley by exactly ![](http://main.edu.pl/images/OI19/wyr-en-tex.1.png) meters;  the other can do the same, i.e., either increase or decrease the  ground level of any connected area in the valley, but by exactly ![](http://main.edu.pl/images/OI19/wyr-en-tex.2.png) meters.

Notice that neither before such an operation nor after it needs the ground in the affected  area be actually leveled.

Given a map of the area, determine the minimum number of operations required to  level the ground in the whole valley, i.e., to make the ground level everywhere  equal 0.  While the operations are performed, the ground level at any point in  the valley can have arbitrary value; in particular, it may be negative.

## 输入格式
In the first line of the standard input there are three integers, ![](http://main.edu.pl/images/OI19/wyr-en-tex.3.png), ![](http://main.edu.pl/images/OI19/wyr-en-tex.4.png), ![](http://main.edu.pl/images/OI19/wyr-en-tex.5.png)    (![](http://main.edu.pl/images/OI19/wyr-en-tex.6.png), ![](http://main.edu.pl/images/OI19/wyr-en-tex.7.png)), separated by single spaces.

The number ![](http://main.edu.pl/images/OI19/wyr-en-tex.8.png) denotes the valley's length in meters.

The second line contains ![](http://main.edu.pl/images/OI19/wyr-en-tex.9.png) integers, ![](http://main.edu.pl/images/OI19/wyr-en-tex.10.png), separated by single spaces.

These numbers, all with absolute value no larger than ![](http://main.edu.pl/images/OI19/wyr-en-tex.11.png), represent the initial ground level in meters    of successive one meter long slices of the valley.

In tests worth 30% of the points the following conditions hold in addition: ![](http://main.edu.pl/images/OI19/wyr-en-tex.12.png) and   ![](http://main.edu.pl/images/OI19/wyr-en-tex.13.png).

In tests worth 60% of the points the following conditions hold in addition: ![](http://main.edu.pl/images/OI19/wyr-en-tex.14.png) and   ![](http://main.edu.pl/images/OI19/wyr-en-tex.15.png).

In tests worth 90% of the points the condition ![](http://main.edu.pl/images/OI19/wyr-en-tex.16.png) holds in addition.


## 输出格式
In the first and only line of the standard output your program should print a single    integer: the minimum number of operations required to level the ground in the whole valley,    or ![](http://main.edu.pl/images/OI19/wyr-en-tex.17.png) if leveling the whole valley with given excavators is impossible.


## 题目大意
### 题目描述

**译自 POI 2012 Stage 3. Day 1「[Leveling Ground](https://szkopul.edu.pl/problemset/problem/W54iZIwStF1TYWRxa1bdVPQo/site/?key=statement)」**

给定一个长度为 $n$ 的数组，每次操作可以将一个区间的数增加或减少 $a$，或将一个区间的数增加或减少 $b$。求使整个数组变为 $0$ 的最小操作次数。若无解请输出 $-1$。

### 输入格式

第一行三个整数 $n, a, b (1 \le n \le 100\ 000, 1 \le a,b \le 10^9)$。

接下来一行 $n$ 个整数 $h_1, h_2, \ldots, h_n$，绝对值均不超过 $10^9$。

### 输出格式

输出一行一个整数，表示最小操作次数。

### 样例解释

一种操作方案是：
* 将前两个数加 $2$；
* 将前两个数减 $3$；
* 将后四个数加 $2$；
* 将最后一个数加 $2$；
* 将后四个数减 $3$。

### 数据范围

对于 $30\%$ 的数据，$n,a,b \le 200,-200 \le h_1,h_2,\ldots,h_n \le 200$.

对于 $60\%$ 的数据，$n,a,b \le 2000,-2000 \le h_1,h_2,\ldots,h_n \le 2000$.

对于 $90\%$ 的数据，$a,b \le 10^6$.

对于所有数据，$1 \le n \le 100\ 000, 1 \le a,b \le 10^9$.

翻译来自于 [LibreOJ](https://loj.ac/p/2701)。

```input1
5 2 3
1 2 1 1 -1
```

```output1
5
```

