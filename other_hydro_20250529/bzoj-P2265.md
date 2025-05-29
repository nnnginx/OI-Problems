## 题目描述

You're driving your car in the local hills and returning to your home town．You'd like to get back as quickly as possible；however，you notice that you don't have much fuel left．You know the most efficient route to take．Some parts of this route go downhill．and some go uphill．The different parts have different lengths and slopes．How quickly can you reach home with the little fuel you have left？

We will assume a very simple model for the fuel consumption of your car．Fuel consumption（per unit distance travelled）will increase linearly with your driving speed $v$．However，there is an offset which depends on the slope $s$ of the hill．For example，when going downhill along a particular road，you might be able to go at $10$ km/h without expending any fuel；on the other hand,，if you were travelling that same road uphill，you would expend fuel at the same rate as if you were driving $10$ km/h faster along a flat road．More specifically，the car's fuel consumption $c$ in liters per kilometer is given by．
where $α$ is the standard fuel consumption rate on a flat road，$v$ is your speed in km/h，$s$ is the slope of the road，and $β$ is a positive constant．Acceleration and deceleration do not cost fuel and can be done instantaneously．

Note that your car has a maximum （safe） speed which cannot be exceeded．

<center>$c ＝ max$ （$0$，$α \cdot v ＋ β \cdot s$）</center>


$α$ **是在平路上的油耗，**$v$ **是速度，**$s$ **是坡度，**$β$ **是个常数。**

**加速减速不耗能量。你的车是有极速的。不可超越**

## 输入格式

On the first line a positive integer：the number of test cases，at most $100$．After that per test case：

One line with four floating point numbers $α，β，vmax$ and $f$：the standard（flat road） fuel consumption rate of your car，the slope factor，the maximum speed of your car in km/h，and the amount of fuel you have left in liters，respectively．

One line with an integer $r$：the number of road segments．

$r$ lines with two floating point numbers $x_i$ and $y_i$ each：the horizontal distance and height change（both in meters）of the $i$-th road segment．Each road segment has constant slope．

**第一行给出** $α，β，vmax$ **和** $f$**。**
**表示的是上式的** $α，β$ **，极速和油量。**
**然后是** $r$**，表示** $r$ **段路程。**
**然后给出** $r$ **个点，表示水平距离和垂直高度。每个坡斜率相同。**

## 输出格式

Per test case：

One line with a floating point number：the fastest time in hours in which you can reach town．It is guaranteed that if it is possible to reach town at all，it will always be possible in less than $24$ hours．If it is impossible to reach town，the line must contain `IMPOSSIBLE` instead．

Your output should have a relative or absolute error of at most $10^{−6}$．

**最快到达终点的时间。达不到就写 `IMPOSSIBLE`**。

```input1
3
10.0 1.0 150 0.0
1
100.0 -100.0
10.0 100.0 150 1.0
2
100 0
100 100
0.5 0.1 100 10
3
1000 0
100 10
100 -10
```

```output1
1.414214
IMPOSSIBLE
0.072120
```

## 数据规模与约定

$100\%$ 的数据满足：$0.1 \le α,β \le 100$，$10 \le vmax \le 200$，$0 \le f \le 50$，$1 \le r \le 1 \times 10^4$，$1 \le x_i \le 1 \times 10^3$，$−1 \times 10^3 \le y_i \le 1 \times 10^3$。