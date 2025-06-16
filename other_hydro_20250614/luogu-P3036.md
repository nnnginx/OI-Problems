## 题目描述
For some reason, Farmer John's cows always seem to be running laser light shows.

For their latest show, the cows have procured a large powerful laser -- so large,in fact, that they cannot seem to move it easily from the location where it was delivered. They would like to somehow send the light from the laser to the barn on the other side of FJ's property.  Both the laser and the barn can be considered to be located at points in the 2D plane on a map of FJ's farm.  The cows plan to point the laser so that it sends a beam of light out either horizontally or vertically (i.e.,  aligned with the x or y axes).  They will then bounce this beam off a number of mirrors to direct it to the barn.

On the farm there are $N$ fence posts ($1 \leq N \leq 100,000$) located at distinct 2D points (also distinct from the laser and the barn) at which the cows can mount mirrors.  The cows can choose not to mount a mirror on a fence post, in which case the laser would simply pass straight over the top of the post without changing direction.  If the cows do mount a mirror on a fence post, they align it diagonally like / or \ so that it will re-direct a horizontal beam of light in a vertical direction or vice versa.

Please compute the minimum possible number of mirrors the cows need to use in order to re-direct the laser to the barn.


## 输入格式
The first line of input contains 5 space-separated integers: $N, x_L, y_L, x_B, y_B$, where $(x_L, y_L)$ is the location of the laser and $(x_B, y_B)$ is the location of the barn.  All coordinates are between $0$ and $1,000,000,000$.

The next $N$ lines each contain the $x$ and $y$ locations of a fence post, both integers in the range $0 \ldots 1,000,000,000$.

## 输出格式
Please output the minimum number of mirrors needed to direct the laser to the barn, or -1 if this is impossible to do.

## 题目大意
### 题目描述

出于某种原因，Farmer John 的奶牛似乎总是在举办激光表演。

在它们的最新表演中，奶牛们获得了一台大型强力激光器——事实上，这台激光器太大，以至于它们无法轻易从交付地点移动它。它们希望以某种方式将激光器的光束发送到 Farmer John 的农场另一边的谷仓。激光器和谷仓都可以被视为位于 Farmer John 农场地图的二维平面中的点。奶牛们计划将激光器指向水平或垂直方向（即与 $x$ 轴或 $y$ 轴对齐），然后通过多次反射镜将光束引导到谷仓。

农场上有 $N$ 个栅栏柱（$1 \leq N \leq 100,000$），位于与激光器和谷仓不同的二维点上，奶牛们可以在这些栅栏柱上安装反射镜。奶牛们可以选择不在栅栏柱上安装反射镜，在这种情况下，激光器会直接穿过栅栏柱而不改变方向。如果奶牛们在栅栏柱上安装反射镜，它们会将其对角线对齐，例如 / 或 \，以便将水平光束重新定向为垂直方向，反之亦然。

请计算奶牛们将激光器引导到谷仓所需的最少反射镜数量。

### 输入格式

输入的第一行包含 $5$ 个用空格分隔的整数：$N, x_L, y_L, x_B, y_B$，其中 $(x_L, y_L)$ 是激光器的位置，$(x_B, y_B)$ 是谷仓的位置。所有坐标都在 $0$ 到 $1,000,000,000$ 之间。

接下来的 $N$ 行每行包含一个栅栏柱的 $x$ 和 $y$ 位置，这两个整数都在 $0 \ldots 1,000,000,000$ 范围内。

### 输出格式

请输出将激光器引导到谷仓所需的最少反射镜数量，如果无法实现，则输出 -1。

```input1
4 0 0 7 2
3 2
0 2
1 6
3 0
```

```output1
1
```

