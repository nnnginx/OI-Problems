## 题目描述
Figuring that they cannot do worse than the humans have, Farmer John's cows have decided to start an airline. Being cows, they decide to cater to the heretofore-untapped market of cows as passengers. They plan to serve the cows who live along the western coast of Lake Michigan. Each morning, they will fly from the northern-most point of the coast southward towards Chicowgo, making many stops along the way. Each evening, they will fly back north to the northernmost point. They need your help to decide which passengers to carry each day. Each of $n \ (1 \le  n \le  10^4)$ farms numbered $1\dots n$ along the coast contains an airport (Farm $1$ is northern-most;farm $n$ is southern-most). On this day,$k \ (1 \le  k \le  5\times 10^4)$ groups of cows wish to travel. Each group of cows wants to fly from a particular farm to another particular farm. The airline, if it wishes, is allowed to stop and pick up only part of a group. Cows that start a flight, however, must stay on the plane until they reach their destination. Given the capacity $c \ (1 \le  c \le  100)$ of the airplane and the groups of cows that want to travel, determine the maximum number of cows that the airline can fly to their destination.

为了表示不能输给人类，农场的奶牛们决定成立一家航空公司。她们计划每天早晨，从密歇根湖湖岸的最北端飞向最南端，晚上从最南端飞往最北端。在旅途中，航空公司可以安排飞机停在某些机场。他们需要你帮助来决定每天携带哪些旅客。沿着湖岸，有 $n$ 个由北至南编号为 $1$ 到 $n$ 的农场。每个农场都有一个机场。这天，有 $k$ 群牛想要乘坐飞机旅行。每一群牛想要从一个农场飞往另一个农场。航班可以在某些农场停下带上部分或全体的牛。奶牛们登机后会一直停留直至达到目的地提供给你飞机的容量 $c$，同时提供给你想要旅行的奶牛的信息，请你计算出这一天的航班最多能够满足几只奶牛的愿望。

## 输入格式
* Line $1$: Three space-separated integers: $k,n$, and $c$.
* Lines $2\dots k+1$: Each line contains three space-separated integers $s,e$, and $m$ that specify a group of cows that wishes to travel. The $m \ (1 \le  m \le  c)$ cows are currently at farm $s$ and want to travel to farm $e \ (s \neq e)$.
* 第一行：$3$ 个用空格隔开的整数 $k$，$n$ 和 $c$。
* 第二到 $k+1$ 行：每一行有 $3$ 个用空格隔开的整数 $s$，$e$，$m$。 表示有 $m$ 只奶牛想从农场 $s$ 乘飞机到农场 $e$。
## 输出格式
* Line $1$: The maximum number of cows that can be flown to their destination. This is the sum of the number of cows flown to their destination on the flight southward in the morning plus the number of cows flown to their destination on the flight northward in the evening.
* 可以完成旅行的奶牛人数的最大值。

```input1
4 8 3
1 3 2
2 8 3
4 7 1
8 3 2
```

```output1
6
```
## 样例说明

INPUT DETAILS:  
Four groups of cows, eight farms, and three seats on the plane.

$3$ 群想要旅行的奶牛，$8$ 个农场，飞机上有 $3$ 个座位。早晨，飞机把 $2$ 只牛从 $1$ 带到 $3$，$1$ 只牛从 $2$ 带到 $8$，$1$ 只牛从 $4$ 带到 $7$。晚上，航班把 $2$ 只牛从 $8$ 带到 $3$。
## 数据规模与约定
对于 $100\%$ 的数据，$1 \le  n \le  10^4$，$1 \leq k \leq 5\times 10^4$，$1 \leq m \leq c \leq 100$。
## 题目来源
Gold