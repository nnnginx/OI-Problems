## 题目描述
Tired of the cold winter weather on her farm, Bessie the cow plans to fly to a warmer destination for vacation. Unfortunately, she discovers that only one airline, Air Bovinia, is willing to sell tickets to cows, and that these tickets are somewhat complicated in structure.

Air Bovinia owns N planes (1 <= N <= 1000), each of which flies on a specific "route" consisting of two or more cities.  For example, one plane might fly on a route that starts at city 1, then flies to city 5, then flies to city 2, and then finally flies to city 8. No city appears multiple times in a route. If Bessie chooses to utilize a route, she can board at any city along the route and then disembark at any city later along the route. She does not need to board at the first city or disembark at the last city. Each route has a certain cost, which Bessie must pay if she uses any part of the route, irrespective of the number of cities she visits along the route. If Bessie uses a route multiple times during her travel (that is, if she leaves the route and later comes back to use it from antoher city), she must pay for it each time it is used.

Bessie would like to find the cheapest way to travel from her farm (in city A) to her tropical destination (city B). Please help her decide what is the minimum cost she must pay, and also the smallest number of individual flights she must use take to achieve this minimum cost.


## 输入格式
The first line of input contains A, B, and N, separated by spaces.

The next 2N lines describe the available routes, in two lines per route. The first line contains the cost of using the route (an integer in the range 1..1,000,000,000), and the number of cities along the route (an integer in the range 1..100).  The second line contains a list of the cities in order along the route.  Each city is identified by an integer in the range 1..1000. Note that the cost of an itinerary can easily add up to more than can fit into a 32-bit integer, so you should probably use 64-bit integers (e.g., "long long" integers in C/C++).


## 输出格式
Output the minimum cost of an itinerary that Bessie can use to travel from city A to city B, as well as the minimum number of individual flights required to achieve this minimum cost. If there is no solution, output "-1 -1" (quotes for clarity) on a single line.


## 题目大意
### 题目描述

Bessie 对她农场那寒冷的天气感到厌烦，于是她准备坐飞机到一个更温暖的地方度假。不幸的是，她发现只有一个航空公司：Air Bovinia，愿意卖票给牛，并且这些票的结构有些复杂。

Air Bovinia 拥有 $n$ 架飞机，每架飞机都有一个经过两个及以上的城市的特殊航线。举个例子：一架飞机可以从城市 $1$ 出发，然后飞往城市 $5$，再飞到城市 $2$，最后飞到城市 $8$。注意**航线是单向的**。任何城市都不会在同一条航线上出现多次。如果 Bessie 选择了一条航线，那么她可以从航线上的任意一个城市上飞机，然后在途中任意一个城市下飞机。他不必从航线的起点上飞机，再从航线的终点下飞机。每条航线都有一个确定的花费，只要它搭乘了这个航班，她就必须支付这个航班的全额花费，不论她途经了几个城市。如果 Bessie 多次搭乘了某个航班，那么每次搭乘 Bessie 都必须支付航班的花费。

Bessie 想要找到从她农场所在的城市（城市 $A$）到她目的地所在城市（城市 $B$）最便宜的路线。请你告诉她他最少要花多少钱，并告诉她在此基础上她最少要**经过几段航线**，也即经过的城市数量 $-1$（包括起点和终点）。

### 输入格式

第一行三个整数 $A,B,n$。

接下来 $2n$ 行，每两行描述一次航班。第一行包括航线的花费 $cost$ 与经过的城市数 $len$。第二行 $len$ 个整数，表示航班依次经过的城市。

### 输出格式

一行两个整数，输出 Bessie 旅行最少要花的钱以及在此基础上最少的经过航线数量。

如果 Bessie 不能从她的农场到达她的目的地，则输出 `-1 -1`。

### 数据范围

$1\le n\le 1000$，$1\le cost\le 10^9$，$1\le len\le 100$。城市的编号均不超过 $1000$。

可能需要开 `long long`。


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

