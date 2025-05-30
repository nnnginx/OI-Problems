## 题目描述

在世界末日的前一天，所有神牛全部来到了一个矩形大广场上。这让你——一个相对还很弱小的同学感到透不过气来，因为神牛会产生看不到的气场，让人身心俱疲。

具体的，每个神牛的控制区域都是一条线段 $(x_1,y_1)\rightarrow (x_2,y_2)$，两端点有可能相同，那样就变成了一个点。

设你所在的位置为点 $P$，如果可以过 $P$ 做两条互相垂直的直线，使得这两条直线都与某一个或某两个神牛的控制区域有公共点，那么这个 $P$ 点就是被气场覆盖的部分，这是你不想呆在的地方，你只想一个人静一静，于是，你想知道这个广场的安静系数的值。其中，安静系数 $=$ 未被气场覆盖的面积 $\div$ 广场总面积。

## 输入格式

输入的第一行包含三个整数 $n,X,Y$，分别表示神牛的个数，以及广场的长和宽。广场的区域范围为 $(0,0)\sim (X,Y)$。

接下来 $n$ 行，每行有四个用空格隔开的非负整数 $x_1,y_1,x_2,y_2$，表示该神牛的控制线段为 $(x_1,y_1)\rightarrow (x_2,y_2)$，其中，$x_1,x_2$ 在 $0$ 到 $X$ 之间，$y_1,y_2$ 在 $0$ 到 $Y$ 之间.

## 输出格式

输出一个 $0$ 到 $1$ 之间的数，表示这个广场的安静系数，只要输出的答案和参考答案相差不超过 $0.005$ 就算正确。

## 样例输入

```plain
1 2 2
0 1 2 1
```

## 样例输出

```plain
0.214602
```

## 样例说明

实际上，样例对应的气场覆盖的区域为以 $(1,1)$ 为圆心的一个圆，面积为 $\pi$，而安静系数自然就等于 $(4-\pi)\div 4=0.2146018\dots$

## 数据规模与约定

$100\%$ 的数据满足，$n\leq 50,X\leq 1\times 10^4,Y\leq 100$。

## 提示

鸣谢 Benz 提供 spj 程序！（修者按：本 OJ 上的 SPJ 由修缮本题面者提供。）
