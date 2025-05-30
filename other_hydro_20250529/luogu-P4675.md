## 题目描述
In the capital of Byteland, there is a fenced park whose area is a rectangle. The trees and the visitors in the park are represented as circles.

There are four entrances in the park, one in each corner (1 = bottom-left, 2 =bottom-right, 3 = top-right, 4 = top-left). The visitors can enter and exit the park only through the entrances.

Visitors can enter and exit the park when they touch both sides of a corner of the corresponding entrance. Visitors can move freely in the park, but they cannot overlap any of the trees or the fence.

Your task is to calculate for each visitor, given the entrance they will enter the park,through which entrances they can exit the park.

## 输入格式
The first input line contains two integers $w$ and $h$ : the number of trees in the park and the number of visitors.

The second input line contains two integers $w$ and $h$ : the width and the height of the park area. The bottom-left corner is $(0,0)$, and the top-right corner is $(w,h)$.

After this, there are  lines that describe the trees. Each line contains three integers, $x,y$ and $r$ : the center of the tree is $(x,y)$ and its radius is $r$. The trees do not overlap each other or the fence.

Finally, there are $m$ lines that describe the visitors. Each line contains two integers $r$ and $e$ : the radius of the visitor and the entrance they will enter the park.

In addition, no tree overlaps a square area of $2k\times2k$ in each corner, where $k$ is the radius of the largest visitor.

## 输出格式
You should output for each visitor a single line containing the entrances through which they can exit the park, in sorted order without spaces in between.

## 题目大意
## 题目描述

在 Byteland 的首都，有一个以围墙包裹的矩形公园，其中以圆形表示游客和树。  
公园里有四个入口，分别在四个角落（$1, 2, 3, 4$ 分别对应左下、右下、右上、左上）。游客只能从入口进出。  
游客可以在他们与公园的两邻边相切的时候进出对应的入口。游客可以在公园里自由活动但不允许与树重叠。  
你的任务是为每个游客计算，给定他们进入公园的入口，他们可以从哪个入口离开公园。

## 输入格式

第一行包含两个整数 $n$ 和 $m$，分别为树的个数和游客的个数。  
第二行包含两个整数 $w$ 和 $h$，公园的左下角在 $(0,0)$，右上角在 $(w,h)$。  
接下来 $n$ 行，每行三个整数 $x,y$ 和 $r$，表示有一棵圆心在 $(x,y)$ 且半径为 $r$ 的树。保证树与树之间不会互相重叠。  
接下来 $m$ 行，每行两个整数 $r$ 和 $e$，表示有一个半径为 $r$ 的游客从入口 $e$ 进入。  
此外，保证没有树会与每个角落的一个大小为 $2k^2$ 的方形区域重叠，$k$ 表示最大的游客半径。

## 输出格式

对于每个游客，输出没有空格的一行，表示该游客可以从这几个入口离开，按照升序排列。

## 限制与提示

两个物体有重叠定义为它们不止一个公共点。

下图展示了每个游客的入口和可能的路线：

![](https://i.loli.net/2018/08/11/5b6e30c4b5a35.png)

对于每个子任务，$4k \leq w,h \leq 10^9$，$k$表示最大的游客半径。

|子任务|分数|数据范围|
|:-:|:-:|-|
|1|27|$1 \leq n \leq 2000,m=1$|
|2|31|$1 \leq n \leq 200,1 \leq m \leq 10^5$|
|3|42|$1 \leq n \leq 2000,1 \leq m \leq 10^5$|

由 @I_love_him52 提供翻译

```input1
5 3
16 11
11 8 1
6 10 1
7 3 2
10 4 1
15 5 1
1 1
2 2
2 1

```

```output1
1234
2
14

```

## 提示
Two objects touch if they have one common point. Two objects overlap if they have more than one common point.

## 样例解释

The following figure shows the entrance areas and possible routes for each visitor:

![](https://cdn.luogu.com.cn/upload/pic/20869.png)

## Subtasks

In all subtasks $4k\leq w,h\leq10^9$ where $k$ is the radius of the largest visitor.

### Subtask 1 (27 points)

- $1\leq n\leq2000$

- $m=1$

### Subtask 2 (31 points)

- $1\leq n\leq200$

- $1\leq m\leq10^5$

### Subtask 3 (42 points)

- $1\leq n\leq2000$

- $1\leq m\leq10^5$


