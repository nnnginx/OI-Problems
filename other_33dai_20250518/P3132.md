## 题目描述
Bessie the cow has designed what she thinks will be the next big hit video game: "Angry Cows".  The premise,  which she believes is completely original, is that the player shoots a cow with a slingshot  into a one-dimensional scene consisting of a set of hay bales located at various points on a number line; the cow lands with sufficient force to detonate the hay bales in close proximity to her landing site, which in turn might set of a chain reaction that causes additional hay bales to explode.  The goal is to use a single cow to start a chain reaction that detonates all the hay bales.

There are $N$ hay bales located at distinct integer positions $x_1, x_2, \ldots, x_N$ on the number line.  If a cow is launched with power $R$ landing at position $x$, this will causes a blast of "radius $R$", engulfing all hay bales within the range $x-R \ldots x+R$.  These hay bales then themselves explode (all simultaneously), each with a blast radius of $R-1$.  Any not-yet-exploded bales caught in these blasts then all explode (all simultaneously) with blast radius $R-2$, and so on.

Please determine the minimum amount of power $R$ with which a single cow may be launched so that, if it lands at an appropriate location, it will cause subsequent detonation of every single hay bale in the scene.

## 输入格式
The first line of input contains $N$ ($2 \leq N \leq 50,000$).  The remaining

$N$ lines all  contain integers $x_1 \ldots x_N$ (each in the range $0 \ldots 1,000,000,000$).


## 输出格式
Please output the minimum power $R$ with which a cow must be launched in order to detonate all the hay bales.  Answers should be rounded and printed to exactly 1 decimal point.


## 题目大意
### 题目描述

奶牛 Bessie 设计了一款她认为将成为下一个热门视频游戏的游戏：“愤怒的奶牛”。她认为这个游戏的设定是完全原创的：玩家用弹弓将一头奶牛射入一个一维场景中，场景由数轴上不同位置的干草堆组成；奶牛以足够的力量落地，引爆她着陆点附近的干草堆，这可能会引发连锁反应，导致更多的干草堆爆炸。目标是用一头奶牛引发连锁反应，引爆所有干草堆。

有 $N$ 个干草堆位于数轴上不同的整数位置 $x_1, x_2, \ldots, x_N$。如果一头奶牛以威力 $R$ 被发射到位置 $x$，这将引发一个“半径为 $R$”的爆炸，吞噬 $x-R \ldots x+R$ 范围内的所有干草堆。这些干草堆随后会同时爆炸，每个爆炸的半径为 $R-1$。任何尚未爆炸的干草堆如果被这些爆炸波及，则会同时爆炸，爆炸半径为 $R-2$，依此类推。

请确定发射一头奶牛所需的最小威力 $R$，使得如果它落在适当的位置，将引发所有干草堆的爆炸。

### 输入格式

输入的第一行包含 $N$（$2 \leq N \leq 50,000$）。接下来的 $N$ 行每行包含一个整数 $x_1 \ldots x_N$（每个整数都在 $0 \ldots 1,000,000,000$ 范围内）。

### 输出格式

请输出发射奶牛所需的最小威力 $R$，以便引爆所有干草堆。答案应四舍五入并精确到小数点后一位。

### 说明/提示

在这个例子中，一头奶牛以威力 $3$ 发射到位置 $5$，将立即引爆位置 $3$ 和 $8$ 的干草堆。这些干草堆随后同时爆炸，每个爆炸的半径为 $2$，吞噬位置 $1$ 和 $10$ 的干草堆，这些干草堆接下来同时爆炸，爆炸半径为 $1$，吞噬位置 $11$ 的最后一个干草堆，该干草堆最终以爆炸半径 $0$ 爆炸。

```input1
5
8
10
3
11
1
```

```output1
3.0
```

## 提示
In this example, a cow launched with power 3 at, say, location 5, will cause immediate detonation of  hay bales at positions 3 and 8. These then explode (simultaneously) each with blast radius 2, engulfing bales at positions 1 and 10, which next explode (simultaneously) with blast radius 1, engulfing the final bale at position 11, which finally explodes with blast radius 0.

