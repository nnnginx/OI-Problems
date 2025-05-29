## 题目描述
Farmer John has installed a fancy new milking machine in his barn, but it draws so much power that it occasionally causes the power to go out! This happens so often that Bessie has memorized a map of the barn, making it easier for her to find the exit of the barn in the dark. She is curious though about the impact of power loss on her ability to exit the barn quickly. For example, she wonders how much farther she might need to walk find the exit in the dark.

The barn is described by a simple (non self-intersecting) polygon with integer vertices $(x_1,y_1)\ldots(x_n,y_n)$ listed in clockwise order. Its edges alternate between horizontal (parallel to the x-axis) and vertical (parallel to the y-axis); the first edge can be of either type. The exit is located at $(x_1,y_1)$. Bessie starts inside the barn located at some vertex $(x_i,y_i)$ for $i \gt 1$. She can walk only around the perimeter of the barn, either clockwise or counterclockwise, potentially changing direction any time she reaches a vertex. Her goal is to travel a minimum distance to reach the exit. This is relatively easy to do with the lights on, of course, since she will travel either clockwise or counterclockwise from her current location to the exit -- whichever direction is shorter.

One day, the lights go out, causing Bessie to panic and forget which vertex she is standing at. Fortunately, she still remembers the exact map of the barn, so she can possibly figure out her position by walking around and using her sense of touch. Whenever she is standing at a vertex (including at her initial vertex), she can feel whether it is a left turn or a right turn, and she can tell if that vertex is the exit. When she walks along an edge of the barn, she can determine the exact length of the edge after walking along the entire edge. In general, Bessie will strategically feel her way around her starting vertex until she knows enough information to determine where she is, at which point she can easily figure out how to get to the exit by traveling a minimum amount of remaining distance.

Please help Bessie determine the smallest possible amount by which her travel distance will increase in the worst case (over all possibilities for her starting vertex) for travel in the dark versus in a lit barn, assuming she moves according to an optimal strategy in each case. An "optimal" strategy for the unlit case is one that minimizes this extra worst-case amount.

## 输入格式
The first line of the input contains $N$ ($4 \leq N \leq 200$). Each of the next $N$ lines contains two integers, describing the points $(x_i,y_i)$ in clockwise order around the barn. These integers are in the range $-100,000 \ldots 100,000$.

## 输出格式
Please output the smallest possible worst-case amount by which Bessie's optimal distance in the dark is longer than her optimal distance in a lit barn, where the worst case is taken over all possible vertices at which Bessie can start.

## 题目大意
### 题目描述

农夫约翰在他的谷仓里安装了一台新的挤奶机，但它耗电量太大，偶尔会导致停电！这种情况发生得如此频繁，以至于贝茜已经记住了谷仓的地图，这帮助她在黑暗中更容易找到出口。但她好奇停电会对她快速离开谷仓的能力产生多大影响。例如，她想知道在黑暗中寻找出口可能需要多走多少路。

谷仓由一个简单（无自交）多边形描述，其顶点按顺时针顺序排列为 $(x_1,y_1)\ldots(x_n,y_n)$。多边形的边在水平（平行于 $x$ 轴）和垂直（平行于 $y$ 轴）之间交替；第一条边可以是任意类型。出口位于 $(x_1,y_1)$。贝茜从某个顶点 $(x_i,y_i)$（$i > 1$）开始位于谷仓内部。她只能沿着谷仓的周边行走，可以顺时针或逆时针方向移动，并可在到达顶点时随时改变方向。她的目标是以最短距离到达出口。在有灯光的情况下这很容易，因为她只需从当前位置沿顺时针或逆时针中选择较短的方向行进即可。

某天停电时，贝茜因恐慌而忘记了自己所在的起始顶点。幸运的是，她仍清楚记得谷仓的地图，因此她可能通过行走并利用触觉来确定自己的位置。每当她站在一个顶点时（包括初始顶点），她可以感知该顶点是左转还是右转，并能判断该顶点是否是出口。当她沿着谷仓的边行走时，她可以在走完整条边后确定该边的精确长度。贝茜将策略性地探索周围环境，直到获得足够信息来确定自己的位置，之后她就能轻松计算出剩余的最短路径。

请帮助贝茜计算：在最优策略下，黑暗中最坏情况（考虑所有可能的起始顶点）下她的行走距离相比有灯光时可能增加的最小额外距离。这里的“最优策略”指能最小化这种最坏情况额外距离的策略。

### 输入格式

输入第一行包含 $N$（$4 \leq N \leq 200$）。接下来 $N$ 行每行包含两个整数，按顺时针顺序描述多边形顶点 $(x_i,y_i)$。这些整数的范围在 $-100,000$ 到 $100,000$ 之间。

### 输出格式

请输出在最优策略下，贝茜在黑暗中最坏情况（考虑所有可能的起始顶点）下的行走距离相比有灯光时可能增加的最小额外距离。

### 说明/提示

在此示例中，贝茜可以感知到自己初始位于一个内角处，但由于所有角都是内角，这提供的信息有限。

一种最优策略是始终顺时针行走。如果她从顶点 3 或 4 出发，这是最优选择；如果从顶点 2 出发，则只会增加 2 单位距离。

```input1
4
0 0
0 10
1 10
1 0
```

```output1
2
```

## 提示
In this example, Bessie can feel that she is initially standing at an inward bend, however since in this example all corners are inward bends this tells her little information.

One optimal strategy is to just travel clockwise. This is optimal is she starts at vertex 3 or 4 and only adds 2 units of distance if she starts at vertex 2.

