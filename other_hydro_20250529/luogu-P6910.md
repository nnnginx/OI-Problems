## 题目描述
 ![](https://vj.z180.cn/ba87a214c6b94e2e93a88f7b226c2064?v=1602042036)  

Your hometown has hired some contractors – including you! – to manage its municipal pipe network. They built the network, at great expense, to supply Flubber to every home in town. Unfortunately, nobody has found a use for Flubber yet, but never mind. It was a Flubber network or a fire department, and honestly, houses burn down so rarely, a fire department hardly seems necessary. 

In the possible event that somebody somewhere decides they want some Flubber, they would like to know how quickly it will flow through the pipes. Measuring its rate of flow is your job.

You have access to one of the pipes connected to the network. The pipe is $l$ meters long, and you can start the flow of Flubber through this pipe at a time of your choosing. You know that it flows with a constant real-valued speed, which is at least $v_1$ meters/second and at most $v_2$ meters/second. You want to estimate this speed with an absolute error of at most $\frac{t}{2}$ meters/second.

Unfortunately, the pipe is opaque, so the only thing you can do is to knock on the pipe at any point along its length, that is, in the closed real-valued range $[0,l]$. Listening to the sound of the knock will tell you whether or not the Flubber has reached that point. You are not infinitely fast. Your first knock must be at least $s$ seconds after starting the flow, and there must be at least $s$ seconds between knocks.

Determine a strategy that will require the fewest knocks, in the worst case, to estimate how fast the Flubber is flowing. Note that in some cases the desired estimation might be impossible (for example, if the Flubber reaches the end of the pipe too quickly).

## 输入格式
The input consists of multiple test cases. The first line of input contains an integer $c$ ($1 \leq c \leq 100$), the number of test cases. Each of the next $c$ lines describes one test case. Each test case contains the five integers $l$, $v_1$, $v_2$, $t$ and $s$ ($1 \leq l, v_1, v_2, t, s \leq 10^9$ and $v_1 < v_2$), which are described above.

## 输出格式
For each test case, display the minimal number of knocks required to estimate the flow speed in the worst case. If it might be impossible to measure the flow speed accurately enough, display impossible instead.

## 题目大意
### **题目描述**

你的家乡雇了一些承包商——包括你！—— 来管理市政管道网络。他们花费巨资建设了该网络，以向城镇中的每个家庭供应弹力胶。不幸的是，目前还没有人找到弹力胶的用途，但没关系。这要么是一个弹力胶网络，要么是一个消防部门。但老实说，房屋很少烧毁，似乎并不需要消防部门。

假设某个地方有人决定要制作一些弹力胶，他们希望知道它会在管道中以多快的速度流动。测量它的流动速度就是你的工作。

你可以访问与网络连接的其中一根管道。该管道长度为 $l$ 米，并且你可以在选择的时间开始通过此管道传输弹力胶。你知道它以恒定的实数速度流动，该速度至少为 $v_1$ 米/秒，最多为 $v_2$ 米/秒。你希望以至多 $\frac{t}{2}$ 米/秒的绝对误差估计此速度(即绝对误差不大于 $\frac {t}{2}$)。

不幸的是，管道是不透明的，所以你唯一能做的事就是在管道的任意一点敲打，即在闭合的实数范围 $[0,l]$ 内。通过听到敲打声，你可以知道弹力胶是否到达了那个点。你的速度并不是无限快的。你第一次敲打必须在开始流动后至少 $s$ 秒，并且敲打之间必须有至少 $s$ 秒的间隔。

你的任务是确定一种策略，需要在最坏情况下用最少的敲击来估算弹力胶的流速。注意，在某些情况下，所需的估计可能是不可能的（例如，弹力胶可能过快地到达管道的末端）。

### **输入格式**

输入包含多组数据。输入的第一行包含一个整数 $c$ $(1 \le c \le 100)$，表示数据组数。接下来的 $c$ 行描述了每组数据。每组数据包含五个整数 $l$，$v_1$，$v_2$ ，$t$ 和 $s$ $（1 \le l, v_1, v_2, t, s \le 10^9 \text{并且}v_1<v_2)$，含义如上所述。

### **输出格式**

对于每组数据，输出在最坏情况下估计流速所需的最小敲击次数。如果无法准确测量流速，则输出 "$impossible$"(不含引号)。

### 说明/提示

时间限制：$1000$ ms，空间限制：$1048576$ kB。

### 题目来源

> International Collegiate Programming Contest (ACM-ICPC) World Finals 2015

> [icpc2015.pdf](https://icpc.global/worldfinals/problems/2015-ICPC-World-Finals/icpc2015.pdf)

```input1
3
1000 1 30 1 1
60 2 10 2 5
59 2 10 2 5

```

```output1
5
3
impossible

```

## 提示
Time limit: 1000 ms, Memory limit: 1048576 kB. 

 International Collegiate Programming Contest (ACM-ICPC) World Finals 2015

