## 题目描述
Jacob likes to play with his radio-controlled aircraft. The weather today is pretty windy and Jacob has to plan flight carefully. He has a weather forecast — the speed and direction of the wind for every second of the planned flight.

The plane may have airspeed up to $v_{\max}$ units per second in any direction. The wind blows away plane in the following way: if airspeed speed of the plane is $(v_x, v_y)$ and the wind speed is $(w_x, w_y)$, the plane moves by $(v_x+w_x, v_y+w_y)$ each second.

![](https://cdn.luogu.com.cn/upload/image_hosting/2uyb1zpd.png)

Jacob has a fuel for exactly $k$ seconds, and he wants to learn, whether the plane is able to fly from start to finish in this time. If it is possible he needs to know the flight plan: the position of the plane after every second of flight.

## 输入格式
The first line of the input file contains four integers $S_x, S_y, F_x, F_y$ — coordinates of start and finish ($−10 000 ≤ S_x, S_y, F_x, F_y ≤ 10 000$).

The second line contains three integers $n, k$ and $v_{\max}$ — the number of wind condition changes, duration of Jacob’s flight in seconds and maximum aircraft speed ($1 ≤ n, k, v_{\max} ≤ 10 000$).

The following $n$ lines contain the wind conditions description. The $i$-th of these lines contains integers $t_i, w_{x_i}$ and $w_{y_i}$ — starting at time $t_i$ the wind will blow by vector $(w_{x_i}, w_{y_i})$ each second ($0 = t_1 < ··· < t_i < t_{i+1} < ··· < k; \sqrt{w_{x_i}^2 + w_{y_i}^2} ≤ v_{\max}$).

## 输出格式
The first line must contain `Yes` if Jacob’s plane is able to fly from start to finish in k seconds, and `No` otherwise.

If it can to do that, the following $k$ lines must contain the flight plan. The $i$-th of these lines must contain two floating point numbers $x$ and $y$ — the coordinates of the position ($P_i$) of the plane after $i$-th second of the flight.

The plan is correct if for every $1 ≤ i ≤ k$ it is possible to fly in one second from $P_{i−1}$ to some point $Q_i$, such that distance between $Q_i$ and $P_i$ doesn’t exceed $10^{−5}$, where $P_0 = S$. Moreover the distance between $P_k$ and $F$ should not exceed $10^{-5}$ as well.

## 题目大意
## 简述

大意就是一架飞机要从起点飞到终点，飞机有最大空速，飞行最大时间，给出风速的变化和风如何影响飞机飞行，求出飞机是否能到达终点，如果能就输出飞机的位置变化。

## 题目描述

雅各布（Jacob）喜欢玩他的无线电摇制飞机。今天的风很大，雅各布必须小心地计划飞行。他有一个天气预报——飞行计划中每秒钟的风速和风向。

飞机每秒在任何方向的空速最大都可以达到 $v_{max}$ 。风吹动飞机的方式如下：如果飞机的空速是 $(v_x,v_y)$ 并且风速是 $(w_x,w_y)$ ，那么飞机每秒将移动 $(v_x+w_x,v_y+w_y)$ 。

![P7069-1](https://cdn.luogu.com.cn/upload/image_hosting/2uyb1zpd.png)

雅各布（Jacob）有一种刚好能使用$k$秒的燃料，他想知道，飞机是否能在这段时间内从起点飞到终点。如果可能的话，他需要知道飞行计划：每飞行一秒后飞机的位置。

## 输入格式

输入文件的第一行有四个整数 $S_x,S_y,F_x,F_y$ ，代表起始位置 $(-10000 \le S_x,S_y,F_x,F_y \le 10000)$ 。

第二行有三个整数 $n,k 和 v_{max}$ ——风况变化的次数，雅各布（Jacob）飞行持续的时间（以秒为单位）和飞机最大空速。

剩下的 $n$ 行是对风向的描述，第 $i$ 行有三个整数 $t_i,w_{xi} 和 w_{yi}$ ——从时间 $t_i$ 开始，风速为每秒 $(w_{xi},w_{yi})$ （一个向量） $(0=t_1< \cdots <t_i<t_{i+1}< \cdots <k; \sqrt{{w^2_{xi}}+{w^2_{yi}}} \le v_{max})$ 。

## 输出格式

如果 $k$ 秒内雅各布（Jacob）的飞机能从起点飞到终点则应输出 `Yes` ，否则输出 `No` 。

如果它能飞到，接下来的 $k$ 行必须包括飞行计划。第 $i$ 行必须包括两个浮点数 $x$ 和 $y$ （保留几位貌似没说）——飞行了第 $i$ 秒的平面位置 $(P_i)$ 。

如果对于每个 $1 \le i \le k$ 都能在一秒内从点 $P_{i-1}$ 飞到某个点 $Q_i$ ，使得 $Q_i$ 和 $P_i$ 间距离不超过 $10^{-5}$ ，其中 $P_0=S$ ，那么这个计划就是正确的。此外 $P_k$ 和 $F$ 间的距离也应不超过 $10^{-5}$ 。

## 说明/提示

时间限制： $2s$ ；内存限制： $256MB$ 

by XYY1411

2020/12/08

```input1
1 1 7 4
2 3 10
0 1 2
2 2 0
```

```output1
Yes
3 2.5
5 2.5
7 4
```

## 提示
Time limit: 2 s, Memory limit: 256 MB.

