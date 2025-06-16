## 题目描述

Tired of the cold winter weather on her farm, Bessie the cow plans to fly to a warmer destination for vacation. Unfortunately, she discovers that only one airline, Air Bovinia, is willing to sell tickets to cows, and that these tickets are somewhat complicated in structure. 

Air Bovinia owns $n$ planes, each of which flies on a specific "route" consisting of two or more cities. For example, one plane might fly on a route that starts at city 1, then flies to city 5, then flies to city 2, and then finally flies to city 8. No city appears multiple times in a route. If Bessie chooses to utilize a route, she can board at any city along the route and then disembark at any city later along the route. She does not need to board at the first city or disembark at the last city. Each route has a certain cost, which Bessie must pay if she uses any part of the route, irrespective of the number of cities she visits along the route. If Bessie uses a route multiple times during her travel (that is, if she leaves the route and later comes back to use it from antoher city), she must pay for it each time it is used. Bessie would like to find the cheapest way to travel from her farm (in city $s$) to her tropical destination (city $t$). Please help her decide what is the minimum cost she must pay, and also the smallest number of individual flights she must use take to achieve this minimum cost.

**翻译：**

Bessie 准备坐飞机从 $s$ 市到 $t$ 市。现在有 $n$ 个航班可供选择。每个航班的航线都经过两个及以上的城市。如果 Bessie 选择了一条航线，那么她可以从航线上任意一座城市上飞机，在途中任意一座城市下飞机。如果她搭乘了某个航班，那么就必须支付这个航班的花费 $c_i$。如果她多次搭乘某个航班，那么**每次搭乘都要支付花费**（类似于乘公交车）。

问：Bessie 从 $s$ 市到 $t$ 市最少要花多少钱，以及在此基础上最少坐几次飞机。

## 输入格式

The first line of input contains $s$, $t$, and $n$, separated by spaces. The next $2\times n$ lines describe the available routes, in two lines per route. The first line contains the cost of using the route $c_i$, and the number of cities along the route $a_i$. The second line contains a list of the cities $d_{i,j}$ in order along the route. Note that the cost of an itinerary can easily add up to more than can fit into a 32-bit integer, so you should probably use 64-bit integers (e.g., "long long" integers in C/C++).

第一行三个正整数 $s,t,n$，表示出发点，终点和航班的数量。

接下来的 $2\times n$ 行，每组两行。

第一行为航班的花费 $c_i$，航班的航线包含的城市数 $a_i$。

第二行为该航班从起点到终点所有城市的序号 $d_{i,j}$。

由于航班花费很贵，你应当使用 $64$ 位的整数。

## 输出格式

Output the minimum cost of an itinerary that Bessie can use to travel from city $s$ to city $t$, as well as the minimum number of individual flights required to achieve this minimum cost. 

If there is no solution, output `-1 -1` (quotes for clarity) on a single line.

输出一行。即 Bessie 的最少花费和在此基础上最少乘坐飞机的次数。如果她无法抵达目的地，输出 `-1 -1`。

```input1
3 4 3
3 5
1 2 3 4 5
2 3
3 5 4
1 2
1 5
```

```output1
2 2
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n \le 10^3$，$1\le c_i \le 10^9$，$1\le a_i \le 100$，$1\le d_{i,j} \le 10^3$。

## 题目来源

Silver