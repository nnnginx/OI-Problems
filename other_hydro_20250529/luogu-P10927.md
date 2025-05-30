## 题目描述
There is a travel agency in Adelton town on Zanzibar island. It has decided to offer its clients, besides many other attractions, sightseeing the town. To earn as much as possible from this attraction, the agency has accepted a shrewd decision: it is necessary to find the shortest route which begins and ends at the same place.  Your task is to write a program which finds such a route.

In the town there are $N$ crossing points numbered from $1$ to $N$ and $M$ two-way roads numbered from $1$ to $M$.  Two crossing points can be connected by multipleroads, but no road connects a crossing point with itself.  Each sightseeingroute is a sequence of road numbers $y_1$, ..., $y_k$, $k>2$. The road $y_i(1\le i\le k-1)$ connects crossing points $x_i$ and $x_{i+1}$, the road $y_k$ connectscrossing points $x_k$ and $x_1$. All the numbers $x_1$,...,$x_k$ should be different.The length of the sightseeing route is the sum of the lengths of all roads onthe sightseeing route, i.e. $L(y_1)+L(y_2)+$...$+L(y_k)$ where $L(y_i)$ is thelength of the road $y_i (1\le i\le k)$.  Your program has to find such a sightseeingroute, the length of which is minimal, or to specify that it is not possible, because there is no sightseeing route in the town.


## 输入格式
The first line of input file TRIP. IN contains two positive integers: the number of crossing points $N \le 100$ and the number of roads $M\le 10000$. Each of the next $M$ lines describes one road. It contains 3 positive integers: the number of its first crossing point, the number of the second one, and the length of the road (a positive integer less than $500$).

## 输出格式
There is only one line in output file TRIP.OUT. It contains either a string 'No solution.' in case there isn't any sightseeing route, or it contains the numbers of all crossing points on the shortest sightseeing route in the order how to pass them (i.e. the numbers $x_1$ to $x_k$ from our definition of a sightseeing route), separated by single spaces. If there are multiple sightseeing routes of the minimal length, you can output any one of them.

## 题目大意
### 题目描述

在桑给巴尔岛的阿德尔顿镇，有一家旅行社。除了许多其他景点外，这家旅行社决定为其客户提供该镇的观光旅游。为了从这个项目中获得尽可能多的收益，旅行社做出了一个精明的决定：需要找到一条始于同一地点并结束于同一地点的最短路线。你的任务是编写一个程序来找到这样的一条路线。

在该镇有 $N$ 个编号为 1 到 $N$ 的交叉点，以及 $M$ 条编号为 1 到 $M$ 的双向道路。两个交叉点可以通过多条道路连接，但没有道路连接同一个交叉点。每条观光路线是由道路编号 $y_1$, ..., $y_k$ 组成的序列，其中 $k > 2$。道路 $y_i (1 \le i \le k-1)$ 连接交叉点 $x_i$ 和 $x_{i+1}$，道路 $y_k$ 连接交叉点 $x_k$ 和 $x_1$。所有的交叉点编号 $x_1$, ..., $x_k$ 应该是不同的。观光路线的长度是该路线所有道路长度的总和，即 $L(y_1)+L(y_2)+...+L(y_k)$，其中 $L(y_i)$ 是道路 $y_i (1 \le i \le k)$ 的长度。你的程序需要找到这样一条观光路线，使其长度最小，或者指明不可能找到这样的路线，因为该镇中没有任何观光路线。

### 输入格式

输入第一行包含两个正整数：交叉点的数量 $N \le 100$ 和道路的数量 $M \le 10000$。接下来的 $M$ 行每行描述一条道路。每行包含三个正整数：第一个交叉点的编号，第二个交叉点的编号，以及道路的长度（小于 500 的正整数）。

### 输出格式

输出只有一行。如果没有任何观光路线，则输出字符串 “No solution.”；否则，输出最短观光路线中所有交叉点的编号，按通过的顺序排列（即从定义中的 $x_1$ 到 $x_k$），编号之间用单个空格分隔，**行末不应有多余空格或者换行符**。如果有多个长度相同的观光路线，可以输出其中任意一条。

```input1
5 7
1 4 1
1 3 300
3 1 10
1 2 16
2 3 100
2 5 15
5 3 20
```

```output1
1 3 5 2

```

```input2
4 3
1 2 10
1 3 20
1 4 30
```

```output2
No solution.
```

