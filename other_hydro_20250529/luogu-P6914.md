## 题目描述
The Arca Carania Mountain national park is opening up for tourist traffic. The national park has a number of sites worth seeing and roads that connect pairs of sites. The park commissioners have put together a set of round tours in the park in which visitors can ride buses to view various sites. Each round tour starts at some site (potentially different sites for different tours), visits a number of other sites without repeating any, and then returns to where it started. At least 3 different sites are visited in each round tour. At least one round tour is possible in the national park.

The park commissioners have decided that, for any given road, all buses will be operated by a single company. The commissioners do not want to be accused of favoritism, so they want to be sure that each possible round tour in the park has exactly the same number of roads assigned to each bus company. They realize this may be difficult to achieve. Thus, they want to learn what numbers of bus companies allow for a valid assignment of companies to roads.

Consider Sample Input 1, which is illustrated in Figure 1. There are a total of three round tours for these sites. Some company is assigned road 1-3. It must also be assigned some road on the round tour 1-2-3-4-1, say 2-3. But then it is assigned to two of the three roads on the round tour 1-2-3-1, and no other company can match this – so there can be no other companies. In Sample Input 2 there is only one round tour, so it is enough to assign the roads of this tour equally between companies.

  ![](https://vj.z180.cn/17b3ab5defe058e1bc8649098ddaa63e?v=1603764959) 

   Figure 1: Sample Input 1. 

## 输入格式
The first line of input contains two integers $n$ ($1 \le n \le 2\, 000$), which is the number of sites in the park, and $m$ ($1 \le m \le 2\, 000$), which is the number of roads between the sites. Following that are $m$ lines, each containing two integers $a_ i$ and $b_ i$ ($1 \leq a_ i < b_ i \leq n$), meaning the sites $a_ i$ and $b_ i$ are connected by a bidirectional road. No pair of sites is listed twice.

## 输出格式
Display all integers $k$ such that it is possible to assign the roads to $k$ companies in the desired way. These integers should be in ascending order.

## 题目大意
### 题目描述

给定一张 $n$ 个点 $m$ 条边的无向图，你需要选择一个颜色种类数 $k$，然后用这 $k$ 种颜色给每条边染色，要求对于图中任意一个简单环，每种颜色的边的数量都相同。求所有可行的 $k$。

保证图无重边，无自环。

### 输入格式

第一行两个正整数 $n, m$（$1\leq n, m\leq 2\times 10 ^ 3$）。

接下来 $m$ 行，每行两个正整数 $x, y$（$1\leq x < y \leq n$），表示一条无向边。

### 输出格式

一行按递增顺序输出所有可行的 $k$，用空格隔开。

```input1
4 5
1 2
2 3
3 4
1 4
1 3

```

```output1
1

```

```input2
6 6
1 2
2 3
1 3
1 4
2 5
3 6

```

```output2
1 3

```

## 提示
Time limit: 2000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2015

