## 题目描述
As a world-famous traveler, Prof. Pang's research interest is to travel as many places as possible in his life.

We have a segment $[0, n]$. There are two travelers on it. The first one is on position $p_1$ with velocity $v_1$ (which means s/he can walk $v_1$ unit on the segment per second). The second one is on position $p_2$ with velocity $v_2$.

From their respective beginning points, travelers can walk on the segment. They cannot walk outside the segment. Whenever they want to change their direction, they can turn around immediately.

Please help Prof. Pang to calculate the minimum  possible time by which every position of the segment is passed by at least one traveler.

## 输入格式
The first line contains one integer $test~(1\le test\le 10000)$ -- the number of test cases.

The $i$-th of the next $test$ lines contains five numbers $n, p_{1, i}, v_{1, i}, p_{2, i}, v_{2, i}$ ($0 < n \le 10000$, $0\le p_{1, i},p_{2, i} \le n$, $0.001 \le v_{1, i},v_{2, i} \le 1000$). All numbers have at most $3$ digits after the decimal point.

## 输出格式
For each test case, we should output one number -- the minimum time that every position of the segment is passed by at least one traveler.

Your answer is considered correct if its absolute or relative error does not exceed $10^{-6}$.

## 题目大意
作为著名的旅行者，Prof. Pang 的研究兴趣是在一生中到尽可能多的地方旅游。

在一条 $[0,n]$ 的线段上有两名旅行者，第一名在位置 $p_1$ 以 $v_1$ （每秒钟可以走 $v_1$ 单位的距离）的速度开始运动，第二名在位置 $p_2$ 以 $v_2$ 的速度开始运动。

从他们分别的起始点出发，旅行者可以在线段上移动，但不可以走出线段。他们可以随时改变自己的方向。

请帮助 Prof. Pang 计算至少需要多少时间，线段上的每个位置都至少被一名旅行者经过。

```input1
2
10000.0 1.0 0.001 9999.0 0.001
4306.063 4079.874 0.607 1033.423 0.847
```

```output1
5001000.0000000000
3827.8370013755
```

