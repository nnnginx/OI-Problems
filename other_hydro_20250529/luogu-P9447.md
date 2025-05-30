## 题目描述
Charlotte the spider sits at the center of her spiderweb, which consists of a series of silken straight strands that go from the center to the outer boundary of the web. Charlotte's web also has bridges, each of which connects two adjacent strands. The two endpoints of a bridge always have the same distance to the center of the spiderweb.

When Charlotte has finished a late-night feasting in the center and wants to retreat to some corner, she walks to the edge on autopilot. To do this, she picks a starting strand, and walks along it until she meets the first bridge on that strand. She will cross the bridge and go to the other strand, and then keeps walking outwards until she meets another bridge. Then she will cross that bridge, and repeat this process, until there are no more bridges on the current strand, and then she will walk to the end of the current strand. Note that Charlotte must cross all the bridges that she meets. Figure I.1 illustrates one path Charlotte could take.

Charlotte's favorite corner to sleep in during the daytime is at the end of strand $s$. For each possible starting strand, she wants to know the minimum number of bridges to add to the original web in order to end at $s$. Charlotte can add a bridge at any point along the strand, as long as the added bridge does not touch any other bridge. The two endpoints of any added bridge must have the same distance to the center of the spiderweb, and the bridge must connect two adjacent strands.

![](https://cdn.luogu.com.cn/upload/image_hosting/7nb4cy7c.png)

Figure I.1: The path starting from strand 4 on the spiderweb in Sample Input 1.

## 输入格式
The first line of input has three integers $n$, $m$, and $s$, where $n$ ($3 \leq n \leq 200000$) is the number of strands, m ($0 \leq m \leq 500000$) is the number of bridges, and $s$ ($1 \leq s \leq n$) is Charlotte's favorite strand. Strands are labeled from $1$ to $n$ in counterclockwise order. Each of the remaining $m$ lines contains two integers $d$ and $t$ describing a bridge, where $d$ ($1 \leq d \leq 10^9$) is the bridge's distance from the center of the spiderweb and $t$ ($1 \leq t \leq n$) is the first strand of the bridge in counterclockwise order. Specifically, if $1 \leq t &lt; n$, then the bridge connects strands $t$ and $t+1$. If $t = n$, then the bridge connects strands $1$ and $n$. All bridge distances $d$ are distinct.

## 输出格式
Output $n$ lines, where the $i^{th}$ line is the minimum number of bridges Charlotte needs to add in order to end at strand $s$ after walking on autopilot from strand $i$.

## 题目大意
有一个蜘蛛网，蜘蛛网包含一个中心点，从中心点放射出的 $n$ 条射线，按逆时针方向从 $1$ 到 $n$ 编号，以及 $m$ 条线段，称为“桥”，每条“桥”连接相邻的两条射线。每一条“桥”都和其连接的两条射线构成以中心点为顶点的等腰三角形。

现有一只蜘蛛从某一条射线的无穷远方向出发向中心点移动。如果在路上遇到了“桥” 的一个端点，蜘蛛会沿桥前往另一个端点到达另一条射线，然后继续往中心点移动。

现在蜘蛛会从 $1-n$ 号的每一条射线出发，并且希望最终经由 $s$ 号射线到达中心点。为了这一目的，可以在任两条射线之间的任意位置添加若干个“桥”。你需要对于 $1-n$ 的每一个出发位置计算最少添加“桥”的数量。注意各个询问之间是独立的，在一个询问中添加的“桥”不会对后续询问造成影响。

$3\le n\le200000$，$0\le n\le 500000$，$1\le s\le n$。

```input1
7 5 6
2 1
4 3
6 3
8 7
10 5

```

```output1
2
1
1
1
0
1
2

```

```input2
4 4 2
1 1
2 2
3 3
4 4

```

```output2
1
1
0
1

```

