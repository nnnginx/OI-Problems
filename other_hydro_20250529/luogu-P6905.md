## 题目描述
The year is 2115. The asteroid communication relay system was set up a decade ago by the Asteroid Communication Ministry. It is running fine except for one small problem – there are too many asteroids! The smaller ones not only keep interfering with the signals from the relay stations but they are also a danger to all the maintenance aircrafts that fly between the stations. These small asteroids must be destroyed! The Interplanetary Coalition to Prevent Catastrophes (ICPC) has been charged with removing these dangerous asteroids and has hired an elite team of hot-shot pilots for the job. Han Duo is the captain of this team of asteroid destroyers. Armed with his missiles, Han flies through the asteroid belt blowing up any asteroid that the ICPC deems a nuisance.

The ICPC is having some unfortunate budgetary problems. One result of this is that Han and his team do not have as many missiles as they would like, so they cannot blow up all the troublesome asteroids. But the asteroids are small and the missiles are powerful. So if two asteroids are near each other and line up properly, it is possible to take out both with a single missile.

Han’s screen displays asteroids as non-rotating two-dimensional simple convex polygons, each of which moves at a fixed velocity. He has decided that the best time to hit two asteroids is when the overlap of the two polygons is at a maximum. For example, Figure 1, which illustrates Sample Input 1, shows two asteroids and snapshots of their subsequent positions at 1-second intervals. The two asteroids start touching after $3$ seconds and the maximum overlap area occurs between $4$ and $5$ seconds.

  ![](https://vj.z180.cn/c0ee84911e97a539823bc119cb23e0d7?v=1603764626) 

   Figure 1: Sample Input 1. Two asteroids with crossing paths. 

Calculating when the maximum overlap occurs for two asteroids requires a bit of programming, but unfortunately Han slept through most of his coding classes at the flight academy. This is where you come in.

## 输入格式
The input consists of two asteroid specifications. Each has the form $n\; x_{1}\; y_{1}\; x_{2}\; y_{2}\; \ldots \; x_{n}\; y_{n}\; v_{x}\; v_{y}$ where $n$ $(3 \le n \le 10)$ is the number of vertices, each $x_{i}, y_{i}$ ($-10\, 000 \le x_{i}, y_{i} \le 10\, 000$) are the coordinates of a vertex of the asteroid on Han’s screen given in clockwise order, and $v_{x}, v_{y}$ ($-100 \le v_{x}, v_{y} \le 100$) are the $x$ and $y$ velocities (in units/second) of the asteroid. The $x_{i}$, $y_{i}$ values specify the location of each asteroid at time $t=0$, and the polygons do not intersect or touch at this time. The maximum length of any side of an asteroid is $500$. All numbers in the input are integers.

## 输出格式
Display the time in seconds when the two polygons have maximum intersection, using the earliest such time if there is more than one. If the two polygons never overlap but touch each other, treat it as an intersection where the common area is zero and display the earliest such time. If the polygons never overlap or touch, display never instead. You should consider positive times only. Your output should have an absolute or relative error of at most $10^{-3}$.

## 题目大意
## 题目背景
今年是2115年。小行星通信中继系统是十年前由小行星通信部建立的。有一个小问题——小行星太多，它们很危险！比较小的小行星不仅不断干扰中继站的信号，而且对在中继站之间飞行的所有维修飞机也是一种危险。这些小行星必须被摧毁！防止危险的星际联盟（ICPC）已被下达移除这些危险的小行星的指令，并请了一支精英团队来完成这项工作。Han Duo 是这个小行星驱逐舰小组的队长。Han Duo 带着他的导弹飞过小行星带，炸毁了 ICPC 认为的令人讨厌的任何小行星。

ICPC 没那么多钱。后果是 Han Duo 和他的团队没有他们想要的那么多导弹，因此他们无法炸毁所有麻烦的小行星。但是小行星很小，导弹也很强大。因此，如果两颗小行星彼此靠近并正确排列，就有可能用一枚导弹将两者都摧毁。

Han Duo 的屏幕将小行星显示为非旋转的二维简单凸多边形，每个多边形都以固定速度移动。他认为撞击两颗小行星的最佳时间是两个多边形的重叠达到最大值时。例如，图1演示了样例输入1，显示了两颗小行星及其后续的位置，间隔1秒。两颗小行星在33秒后开始接触，最大重叠区域出现在44到55秒之间。

图1：样例输入1。两颗有交叉路径的小行星。

计算两颗小行星的最大重叠时间需要计算机来完成，但不幸的是，Han Duo 在飞行学院的大部分程序设计课中都在睡大觉。现在把这个任务交由你。

## 输入格式

输入包括两个小行星规格。每个形式为 $n, x_1, y_1 ,x_2，y_2  $ $… $ $x_n ,y_n ,v_x, v_y$ 其中 $n$$(3$$\le n \le10)$  是顶点的数量，每个 $x_i,y_i(-10000$$\leq x_i,y_i \leq$$1000)$ 在屏幕上按顺时针顺序给出的小行星顶点的坐标，$v_x，v_y(-100 \le v_x,v_y \le 100)$ 是小行星的$x$和$y$速度（单位/秒）$x,y$ 值代表 $t=0$ 时每个小行星的位置，此时多边形不相交或接触。小行星任意一侧的最大长度为 $500$。输入中的所有数字都是整数。

## 输出格式

以秒为单位输出两个多边形具有最大相交的时间，如果存在多个多边形，则使用最早的时间。如果两个多边形从不重叠，而是彼此接触，则将其视为公共面积为零的交点，并输出最早的时间。如果多边形从不重叠或接触，则输出“never”。你应该只考虑确定的时候。输出的绝对或相对的误差应不超过$10^{-3}$。

## 说明/提示

时间限制：2000毫秒，内存限制：1048576 kB。

2015年国际大学生编程大赛（ACM-ICPC）世界总决赛

```input1
6 3 2 2 4 3 6 6 6 7 4 6 2 2 2
4 18 5 22 9 26 5 22 1 -2 1

```

```output1
4.193518

```

```input2
4 0 0 0 2 2 2 2 0 -1 1
4 10 0 10 2 12 2 12 0 1 1

```

```output2
never

```

## 提示
Time limit: 2000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2015
 
spj provider:@[shenyouran](/user/137367).

