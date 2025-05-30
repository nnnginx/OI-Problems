## 题目描述
Who am I? What am I? Why am I? These are all difficult questions that have kept philosophers reliably busy over the past millennia. But when it comes to "Where am I", then, well, modern smartphones and GPS satellites have pretty much taken the excitement out of that question.

To add insult to the injury of newly unemployed spatial philosophers formerly pondering the "where" question, the Instant Cartographic Positioning Company (ICPC) has decided to run a demonstration of just how much more powerful a GPS is compared to old-fashioned maps. Their argument is that maps are useful only if you already know where you are, but much less so if you start at an unknown location.

For this demonstration, the ICPC has created a test area that is arranged as an unbounded Cartesian grid. Most grid cells are empty, but a finite number of cells have a marker at their center (see Figure L.1(a) for an example with five marked cells). All empty grid cells look the same, and all cells with markers look the same. Suppose you are given a map of the test area (that is, the positions of all the markers), and you are placed at an (unknown to you) grid cell. How long will it take you to find out where you actually are? ICPC's answer is clear: potentially a very, very long time, while a GPS would give you the answer instantly. But how long exactly?

![](https://cdn.luogu.com.cn/upload/image_hosting/ydxjurja.png)

Figure L.1: Sample grid and the order in which test subjects explore the grid.

In the trial, test subjects will explore their environment by following an expanding clockwise spiral whose first few steps are shown in Figure L.1(b). The starting cell is labeled "0", and the numbers show the order in which other cells are visited. The test subjects can see a marker only if they are at its grid cell, and they will stop their exploration as soon as they know where they are based on the grid cells that they have seen so far. That means that the observed sequence of empty and marked grid cells could have begun only at a single possible starting position. The grid is unbounded, but the exploration will be finite since once a test subject has seen all markers on the grid, they'll definitely know where they are.

Having hundreds of test subjects literally running in circles can be expensive, so the ICPC figures that writing a simulation will be cheaper and faster. Maybe you can help?

## 输入格式
The input describes a single grid. It starts with a line containing two integers $d_x$ , $d_y$ ($1 \leq d_x, d_y \leq 100$). The following $d_y$ lines contain $d_x$ characters each, and describe part of the test grid. The $i^{th}$ character of the $j^{th}$ line of this grid description specifies the contents of the grid cell at coordinate ($i$, $d_y-j+1$). The character is either '$\texttt{.}$' or '$\texttt{X}$', meaning that the cell is either empty, or contains a marker, respectively.

The total number of markers in the grid will be between $1$ and $100$, inclusive. All grid cells outside the range described by the input are empty.

## 输出格式

In ICPC's experiment, a test subject knows they will start at some position ($x$, $y$) with $1 \leq x \leq d_x$, $1 \leq y \leq d_y$.

Output three lines. The first line should have the expected number of steps needed to identify the starting position, assuming that the starting position is chosen uniformly at random. This number needs to be exact to within an absolute error of $10^{-3}$.

The second line should have the maximum number of steps necessary until one can identify the starting position.

The third line should list all starting coordinates ($x$, $y$) that require that maximum number of steps. The coordinates should be sorted by increasing $y$-coordinates, and then (if the $y$-coordinates are the same) by increasing $x$-coordinates.

## 题目大意
输入描述:

一个单独的网格。它以包含两个整数 dx, dy (1≤dx, dy≤100) 的一行开始。接下来的 dy 行每行包含 dx 个字符，并描述了测试网格的一部分。网格描述的第 i 行第 j 列的字符指定了坐标 (i, dy-j+1) 处网格单元的内容。字符可以为 '.' 或 'X'，分别表示该单元格为空或包含标记。

网格中标记的总数将在1到100之间，包括1和100。输入未包含的网格单元都为空。

输出三行。

第一行应该是估计需要识别起始位置的步骤数，假设起始位置是均匀随机选择的。这个数需要精确到$10^{-3}$的绝对误差。

第二行应该是识别起始位置所需的最大步骤数。

第三行应该列出所有需要最大步骤数的起始坐标(x, y)。坐标应按递增的y坐标排序，如果y坐标相同，则按递增的x坐标排序。

```input1
5 5
....X
.X...
.....
X..X.
..X..

```

```output1
9.960000000
18
(1,4) (4,5)

```

```input2
5 1
..XX.

```

```output2
4.600000000
7
(1,1) (5,1)

```

