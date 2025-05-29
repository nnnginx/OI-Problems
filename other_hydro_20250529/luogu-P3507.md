## 题目描述
Alice and Bob learned the minima game, which they like very much, recently.

The rules of the game are as follows.

A certain number of cards lies on a table, each inscribed with a positive integer.

The players make alternate moves, Alice making the first one.

A move consists in picking an arbitrary positive number of cards from the table.

For such move the player receives a number of points equal to the minimum    of the numbers inscribed on the cards he collected.

The game ends when the last card is removed from the table.

The goal of each player is maximizing the difference between their and their opponent's score.

Alice and Bob have duly noted that there is an optimal strategy in the game.

Thus they are asking you to write a program that, for a given set of cards,    determines the outcome of the game when both players play optimally.

## 输入格式
In the first line of the standard input there is one integer ![](http://main.edu.pl/images/OI17/gra-en-tex.1.png) (![](http://main.edu.pl/images/OI17/gra-en-tex.2.png)) given,      denoting the number of cards.

The second line holds ![](http://main.edu.pl/images/OI17/gra-en-tex.3.png) positive integers ![](http://main.edu.pl/images/OI17/gra-en-tex.4.png) (![](http://main.edu.pl/images/OI17/gra-en-tex.5.png)),      separated by single spaces, that are inscribed on the cards.


## 输出格式
Your program should print out a single line with a single integer to the standard      output - the number of points by which Alice wins over Bob, assuming they both play optimally;      if it is Bob who has more points, the result should be negative.


## 题目大意
### 题目描述

**译自 POI 2010 Stage 3. Day 1「[The Minima Game](https://szkopul.edu.pl/problemset/problem/3buviDQZWLE83AxVhvJJurgU/site/?key=statement)」**

Alice 和 Bob 玩一个游戏。Alice 先手，两人轮流进行操作，每轮一个玩家可以选择若干张牌（至少一张），并获得相当于这些牌上所写数字的最小值的分数，直到没有牌为止。两人都希望自己的分数与对方分数之差最大。若两个玩家都使用最佳策略，求游戏的最终结果。

### 输入格式

第一行有一个整数 $n$，表示牌的数量。

接下来一行有 $n$ 个正整数 $k_1, k_2, ..., k_n$，表示牌上所写的数字。

### 输出格式

输出一行一个整数，表示最终 Alice 的分数与 Bob 分数之差。如果 Bob 的分数更多，你应该输出一个负数。

### 样例解释

Alice 先选择 $3$，得到 $3$ 分。Bob 拿走所有牌并得到 $1$ 分，游戏最后的比分为 $3:1$，因此 Alice 比 Bob 多两分。

### 数据范围

$1\le n\le 10^6$，$1\le k_i\le 10^9$。

翻译来自于 [LibreOJ](https://loj.ac/p/2455)。

```input1
3
1 3 1
```

```output1
2
```

