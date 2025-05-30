## 题目背景
与原题相比，$N$ 的数据范围调整为了 $1\leq N\leq 100000$，其他数据范围并无变化。

## 题目描述
Farmer John has constructed an obstacle course for the cow's enjoyment. The course consists of a sequence of $N$ fences ($1\le N \le 100000$) of varying lengths, each parallel to the x axis. Fence i's y coordinate is i.

The door to FJ's barn is at the origin (marked '`*`' below). The starting point of the course lies at coordinate ($S$,$N$).

```
   +--S--+-+-+
+--+--+--+
    ...
   +--+--+-+
      +--+-+-+
|==|==|==*=|=|=|
-3 -2 -1 0 1 2 3
```

FJ's original intention was for the cows to jump over the fences, but cows are much more comfortable keeping all four hooves on the ground. Thus, they will walk along the fence and, when the fence ends, they will turn towards the x axis and continue walking in a straight line until the hit another fence segment or the side of the barn. Then they decide to go left or right until they reach the end of the fence segment, and so on, until they finally reach the side of the barn and then, potentially after a short walk, the ending point.

Naturally, the cows want to walk as little as possible. Find the minimum distance the cows have to travel back and forth to get from the starting point to the door of the barn.


## 输入格式
- Line 1: Two space-separated integers: $N$ and $S$. ($-100000\le S \le 100000$)
- Line 2~N+1: Each line contains two space-separated integers : $A_i$ and $B_i$ ($-100000\le A_i < B_i \le 100000 $) , the starting and ending x-coordinates of fence segment i. Line 2 describes fence #2; line 3 describes fence #2; and so on. The starting position will satisfy $A_N \le S \le B_N$. Note that the fences will be traversed in reverse order of the input sequence.


## 输出格式
- Line 1: The minimum distance back and forth in the x direction required to get from the starting point to the ending point by walking around the fences. The distance in the y direction is not counted, since it is always precisely $N$.


## 题目大意
### 题意翻译

FJ 有 $N $ 个栅栏布置在坐标系上，第 $i$ 个栅栏为 $(A_i,i)$ 到 $(B_i,i)$ 的一条线段（端点处可以通过）。现在某只牛从 $(S,N)$ 出发，进行这样的移动过程（假设目前位置为 $(x,y)$）：

- 如果 $(x,y)$ 处没有栅栏，那么往下走直到遇到栅栏为止。
- 如果遇到栏杆，那么向左或者向右走到 $(A_y,y)$ 或者 $(B_y,y)$ 为止。
- 如果已经走到了 $x$ 轴上，那么沿着 $x$ 轴走到原点。

求牛移动到原点所需要在 $x$ 轴方向上移动的最小距离。

输入第一行给出 $N$ 和 $S$，随后 $N$ 行给出 $A_i$ 和 $B_i$。

示意图为了美观做了修改，每两个 `+` 中间是一单位距离。

```input1
4 0
-2 1
-1 2
-3 0
-2 1
```

```output1
4
```

