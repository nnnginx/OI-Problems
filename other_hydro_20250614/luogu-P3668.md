## 题目描述
Having become bored with standard 2-dimensional artwork (and also frustrated at others copying her work), the great bovine artist Picowso has decided to switch to a more minimalist, 1-dimensional style.


Although, her paintings can now be described by a 1-dimensional array of colors of length $N$ ($1 \leq N \leq 100,000$), her painting style remains unchanged: she starts with a blank canvas and layers upon it a sequence of "rectangles" of paint, which in this 1-dimensional case are simply intervals. She uses each of the colors $1 \ldots N$ exactly once, although just as before, some colors might end up being completely covered up by the end.


To Picowso's great dismay, her competitor Moonet seems to have figured out how to copy even these 1-dimensional paintings, using a similar strategy to the preceding problem: Moonet will paint a set of disjoint intervals, wait for them to dry, then paint another set of disjoint intervals, and so on. Moonet can only paint at most one interval of each color over the entire process. Please compute

the number of such rounds needed for Moonet to copy a given 1-dimensional Picowso painting.

## 输入格式
The first line of input contains $N$, and the next $N$ lines contain an integer in the range $0 \ldots N$ indicating the color of each cell in the 1-dimensional painting (0 for a blank cell).

## 输出格式
Please output the minimum number of rounds needed to copy this painting, or -1 if this could not have possibly been an authentic work of Picowso (i.e., if she could not have painted it using a layered sequence of intervals, one of each color).


## 题目大意
### 题目描述

伟大的牛艺术家 Picowso 对标准的二维艺术作品感到厌倦（同时也对其他人抄袭她的作品感到沮丧），于是决定转向一种更极简主义的一维风格。

尽管她的画作现在可以用一个长度为 $N$（$1 \leq N \leq 100,000$）的一维颜色数组来描述，但她的绘画风格保持不变：她从一个空白画布开始，并在其上叠加一系列“矩形”颜料，而在这种一维情况下，这些矩形仅仅是区间。她使用每种颜色 $1 \ldots N$ 恰好一次，尽管和以前一样，某些颜色最终可能会被完全覆盖。

令 Picowso 非常沮丧的是，她的竞争对手 Moonet 似乎已经找到了如何复制这些一维画作的方法，使用的策略与之前的问题类似：Moonet 会绘制一组不相交的区间，等待它们干燥，然后再绘制另一组不相交的区间，依此类推。在整个过程中，Moonet 只能为每种颜色绘制最多一个区间。请计算 Moonet 复制给定的一维 Picowso 画作所需的最少轮数。

### 输入格式

输入的第一行包含 $N$，接下来的 $N$ 行每行包含一个范围在 $0 \ldots N$ 的整数，表示一维画作中每个单元格的颜色（0 表示空白单元格）。

### 输出格式

请输出复制这幅画作所需的最少轮数，如果这幅画作不可能是 Picowso 的真实作品（即她无法通过叠加一系列区间、每种颜色一个区间的方式绘制它），则输出 -1。

### 说明/提示

在这个例子中，颜色 1 的区间必须在颜色 4 和 5 的区间之前绘制，因此至少需要两轮。

```input1
7
0
1
4
5
1
3
3
```

```output1
2
```

## 提示
In this example, the interval of color 1 must be painted in an earlier round than the intervals of colors 4 and 5, so at least two rounds are needed.

