## 题目描述
As you know, the ACM ICPC is not the only major sporting event taking place in Russia this year. Several months ago, the 2014 Winter Olympics were held in Sochi, which is about 3 000 km from Ekaterinburg.

In an increasing number of sports, it is not only the ability of the athletes that determines who wins a competition but also their equipment. For example in downhill skiing, having the latest ski technology enables athletes to increase their speeds and improve their turning ability.

You have been hired to determine the effect of the latest ski technology on the ability of skiers to navigate a downhill course. The course contains several target locations, and the skier wants to pass over as many of them as possible. Naturally, the better the ski technology, the easier it will be to do this.

For simplicity, use a two-dimensional coordinate system where the skier starts at position (0,0) and where “downhill” corresponds to the direction of the positive $y$-axis.

Assume the $y$-component of the athlete’s velocity is a constant $v_ y$. The athlete can change speed laterally (in the $x$-direction), but the skiing equipment limits this to a maximal lateral acceleration $a_{max}$. The skier starts with a lateral velocity of 0.

![](https://cdn.luogu.com.cn/upload/image_hosting/us59dhj8.png)

   Figure 1: Downhill ski path passing over three targets 

In Figure 1 (which corresponds to the first sample input), the optimal path passes over three out of four possible targets. If $a_{max}$ were smaller, then the skier might be able to pass over only two or fewer of the targets.

## 输入格式
The input contains a single test case. The first line contains three integers $n$, $v_ y$, and $a_{max}$ ($0 \leq n \leq 250$, $0 < v_ y \leq 10^5$ and $0 \leq a_{max} \leq 10^7$), where $n$ is the number of targets, $v_ y$ is the $y$-component of the skier’s velocity, and $a_{max}$ is the maximum lateral acceleration. Here $v_ y$ is given in meters per hour and $a_{max}$ in meters per hour squared.

Following this are $n$ lines, each containing two integers $x_ i$ and $y_ i$ ($-10^5 \leq x_ i, y_ i \leq 10^5$). These give the coordinates of each target to be visited on the course. All coordinates are given in meters. Targets are numbered 1, 2, ..., $n$ in the order they are given.

## 输出格式
Display the maximal-length sequence of targets that the athlete could pass over on the course in a single run. Display the targets in the order they are visited. If there are multiple maximal-length sequences, display only the lexicographically first one. (So the sequence 2 15 would come before the sequence 10 15.) If the athlete cannot pass over any targets, print Cannot visit any targets instead.

To ensure floating-point stability, you may assume the answer will not change if $a_{max}$ is perturbed by up to 0.1.

## 题目大意
**题目描述**

滑雪运动员进行的一次训练可以看作平面上一条从 $(0, 0)$ 出发的曲线，这条曲线在 $y$ 轴正方向上的**速度**是 $v_y$，由于装备限制，在 $x$ 轴上的**加速度**不得超过 $a_{max}$。滑雪运动员在 $x$ 轴上的速度从 $0$ 开始。

在这一次训练中，滑雪运动员需要经过所有 $n$ 个目标点 $(x_i, y_i)$ 中尽可能多的目标点，现在他希望你通过控制他每一时刻的加速度，实现这个目标。

**输入格式**

第一行三个整数 $n, v_y, a_{max}$ 分别表示目标点数，$y$ 轴速度（米每秒）以及 $x$ 轴加速度上限（米每二次方秒）。

接下来 $n$ 行每行两个整数 $x, y$ 表示目标点的横坐标（米）以及纵坐标（米）。

**输出格式**

按照目标点被经过的顺序输出最长的目标点序列。若有多个可能的答案，输出字典序最小的。若运动员不能经过任意一个目标点，输出 `Cannot visit any targets`。

为了避免浮点误差，你可以假设对 $a_max$ 进行不超过 $0.1$ 的扰动的情况下，答案不变。

**数据范围**

$0\le n\le 250, 0\le v_y\le 10^5
, 0\le a_{max}\le 10^7
, −10^5\le x, y\le 10^5$
, 目标点编号从 1 开始。

~~一句话の题意：输入一些数，输出一些数（或字符串），使输出符合要求。~~

```input1
4 100 400
-100 100
50 200
-100 300
150 300

```

```output1
1 2 4

```

```input2
1 100 100
1000 10

```

```output2
Cannot visit any targets

```

## 提示
Time limit: 2000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2014

