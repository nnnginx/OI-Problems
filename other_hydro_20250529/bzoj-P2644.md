## 题目描述

New labyrinth attraction is open in New Lostland amusement park. The labyrinth consists of $n$ rooms connected by $m$ passages. Each passage is colored into some color $c_{i}$. Visitors of the labyrinth are dropped from the helicopter to the room number $1$ and their goal is to get to the labyrinth exit located in the room number $n$.  
Labyrinth owners are planning to run a contest tomorrow. Several runners will be dropped to the room number $1$. They will run to the room number $n$ writing down colors of passages as they run through them. The contestant with the shortest sequence of colors is the winner of the contest. If there are several contestants with the same sequence length, the one with the ideal path is the winner. The path is the ideal path if its color sequence is the lexicographically smallest among shortest paths.
Andrew is preparing for the contest. He took a helicopter tour above New Lostland and made a picture of the labyrinth. Your task is to help him find the ideal path from the room number $1$ to the room number $n$ that would allow him to win the contest.   

**Note**:  
* A sequence ($a_{1}, a_{2},\dotsb, a_{k}$) is lexicographically smaller than a sequence ($b_{1}, b_{2},\dotsb, b_{k}$) if there exists $i$ such that $a_{i} < b_{i}$, and $a_{j} = b_{j}$ for all $j < i$.

给定无向图（有重边）每条边有一种颜色，边权为 $1$，让你找到从 $1$ 到 $n$ 的最短路，并且经过的边的颜色组成的序列的字典序最小。 

## 输入格式

The first line of the input file contains integers $n$ and $m$ —the number of rooms and passages, respectively. The following m lines describe passages, each passage is described with three integer numbers: $a_{i},b_{i}$,and $c_{i}$ — the numbers of rooms it connects and its color. Each passage can be passed in either direction. Two rooms can be connected with more than one passage, there can be a passage from a room to itself. It is guaranteed that it is possible to reach the room number n from the room number $1$.

## 输出格式

The first line of the output file must contain $k$ — the length of the shortest path from the room number $1$ to the room number $n$. The second line must contain $k$ numbers — the colors of passages in the order they must be passed in the ideal path.

## 样例

```input1
4 6
1 2 1
1 3 2
3 4 3
2 3 1
2 4 4
3 1 1

```

```output1
2
1 3
```

## 数据规模与约定

对于 $100\%$ 的数据，$2 \leq n \leq  1 \times 10^5$， $1 \leq m \leq 2 \times 10^5$，$1 \leq a_{i}, b_{i} \leq n$，$1 \leq c_{i} \leq 10^{9}$。

## 题目来源

Pku3967