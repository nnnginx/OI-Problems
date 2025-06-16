## 题目描述
Farmer John is quite the nature artist: he often constructs large works of art on his farm. Today, FJ wants to construct a giant "field web". FJ's field is large convex polygon with fences along the boundary and fence posts at each of the $n$ corners $(1 \le  n \le  150)$. To construct his field web, FJ wants to run as many ropes as possible in straight lines between pairs of non-adjacent fence posts such that no two ropes cross. There is one complication: FJ's field is not completely usable. Some evil aliens have created a total of $g\ (0 \le  g \le  100)$ grain circles in the field, all of radius $r\ (1 \le  r \le  10^5)$. FJ is afraid to upset the aliens, and therefore doesn't want the ropes to pass through, or even touch the very edge of a grain circle. Note that although the centers of all the circles are contained within the field, a wide radius may make it extend outside of the field, and both fences and fence posts may be within a grain circle. Given the locations of the fence posts and the centers of the circles, determine the maximum number of ropes that FJ can use to create his field web. FJ's fence posts and the circle centers all have integer coordinates $x$ and $y$ each of which is in the range $0\dots 10^6$.

约翰真是一个自然派艺术大师，他常常在他的田地上创作一些巨大的艺术杰作。今天，他想在麦田上创作一幅由绳索构成的巨画。他的麦田是一个多边形，由 $n$ 个篱笆桩和之间的篱笆围成。为了创作他的巨画，他打算用尽量多的数量的绳索，笔直地连接两个不相邻的篱笆桩。但是为了画作的优美，任意两根绳索不得交叉。

约翰有一个难处：一些邪恶的外星人在他的麦田上整出了 $g$ 个怪圈。这些怪圈都有一定的半径 $r$。他不敢惹外星人，所以不想有任何绳索通过这些怪圈，即使碰到怪圈的边际也不行。这些怪圈的圆心都在麦田之内，但一些怪圈可能有部分在麦田之外。一些篱笆或者篱笆桩都有可能在某一个怪圈里。给出篱笆桩和怪圈的坐标，计算最多的绳索数。所有的坐标都是 $[0,10^6]$ 内的整数。
## 输入格式
* Line $1$: Three space-separated integers: $n,g$, and $r$. 
* Lines $2\dots n+1$: Each line contains two space-separated integers that are the $x,y$ position of a fence post on the boundary of FJ's field. 
* Lines $n+2\dots n+g+1$: Each line contains two space-separated integers that are the $x,y$ position of a circle's center inside FJ's field.
 
第 $1$ 行输入三个整数 $n,g,r$。接下来 $n$ 行每行输入两个整数表示篱笆桩的坐标。接下来 $g$ 行每行输入两个整数表示一个怪圈的圆心坐标。

## 输出格式
* Line $1$: A single integer that is the largest number of ropes FJ can use for his artistic creation.

最多的线索数。

```input1
5 3 1
6 10
10 7
9 1
2 0
0 3
2 2
5 6
8 3
```
```output1
1
```
## 样例说明

A pentagonal field, in which all possible ropes are blocked by three grain circles, except for the rope between fenceposts $2$ and $4$.

除了篱笆桩 $2$ 和 $4$ 之间可以连接绳索，其余均会经过怪圈。
## 数据规模与约定
对于 $100\%$ 的数据，$1\le n\le 150$，$0\le g\le 100$，$1\le r\le 10^5$，$x_i,y_i\in [0,10^6]$。
## 题目来源
Gold