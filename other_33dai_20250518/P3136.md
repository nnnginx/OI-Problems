## 题目描述
Farmer John is quite reliable in all aspects of managing his farm, except one: he is terrible at mowing the grass in a timely fashion.   He only manages to move the mowing machine once per day, in fact. On day 1, he starts at position $(x_1, y_1)$ and on day $d$ he mows along a straight segment to the position $(x_d, y_d)$, moving either horizontally or vertically on the 2D map of his farm; that is, either  $x_d = x_{d-1}$, or $y_d = y_{d-1}$.  FJ alternates between horizontal and vertical moves on successive days.


So slow is FJ's progress that some of the grass he mows might grow back before he is finished with all his mowing. Any section of grass that is cut in day $d$ will reappear on day $d + T$, so if FJ's mowing path crosses a path he cut at least $T$ days earlier, he will end up cutting grass at the same point again.  In an effort to try and reform his poor mowing strategy, FJ would like to count the number of times this happens.

Please count the number of times FJ's mowing path crosses over an earlier segment on which grass has already grown back.  You should only count "perpendicular" crossings, defined as a point in common between a horizontal and a vertical segment that is an endpoint of neither.

## 输入格式
The first line of input contains $N$ ($2 \leq N \leq 100,000$) and $T$ ($1 \leq T \leq N$, $T$ even).

The next $N$ lines describe the position of the mower on days $1 \ldots N$.  The $i$-th of these lines contains integers $x_i$ and $y_i$ (nonnegative integers each at most 1,000,000,000).


## 输出格式
Please output a count of the number of crossing points described above, where FJ re-cuts a point of grass that had grown back after being cut earlier.


## 题目大意
### 题目描述

Farmer John 在管理农场的各个方面都相当可靠，除了一件事：他非常不擅长及时修剪草地。事实上，他每天只能移动一次割草机。在第 1 天，他从位置 $(x_1, y_1)$ 开始，在第 $d$ 天，他沿着一条直线段移动到位置 $(x_d, y_d)$，在农场的二维地图上，他要么水平移动，要么垂直移动；也就是说，要么 $x_d = x_{d-1}$，要么 $y_d = y_{d-1}$。FJ 在连续的日子里交替进行水平和垂直移动。

FJ 的进展非常缓慢，以至于在他完成所有修剪之前，一些被他修剪过的草可能会重新长出来。任何在第 $d$ 天被修剪的草会在第 $d + T$ 天重新长出来，因此如果 FJ 的修剪路径与至少 $T$ 天前修剪过的路径交叉，他将再次在同一位置修剪草地。为了尝试改进他糟糕的修剪策略，FJ 想要计算这种情况发生的次数。

请计算 FJ 的修剪路径与之前已经重新长草的路径交叉的次数。你只需计算“垂直”交叉，定义为水平线段和垂直线段之间的共同点，且该点不是任何线段的端点。

### 输入格式

输入的第一行包含 $N$（$2 \leq N \leq 100,000$）和 $T$（$1 \leq T \leq N$，$T$ 为偶数）。

接下来的 $N$ 行描述了割草机在第 $1$ 到第 $N$ 天的位置。第 $i$ 行包含整数 $x_i$ 和 $y_i$（每个为非负整数，且不超过 $1,000,000,000$）。

### 输出格式

请输出上述交叉点的数量，即 FJ 重新修剪已经重新长草的点的次数。

### 说明/提示

在这里，FJ 在第 7 天与他在第 2 天修剪的草地路径交叉，这算作一次。其他交叉点不算。

注意：本题有扩展的限制：每个测试用例 5 秒（Python 和 Java 为 10 秒），内存限制为 512 MB。

```input1
7 4
0 10
10 10
10 5
3 5
3 12
6 12
6 3
```

```output1
1
```

## 提示
Here, FJ crosses on day 7 a segment of grass he cut on day 2, which counts. The other intersections do not count.

Note: This problem has expanded limits: 5 seconds per test case (10 for Python and Java), and 512 MB of memory.


