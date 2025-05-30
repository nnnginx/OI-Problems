## 题目描述
In order to make a few dollars, you have decided to become part of a scientific experiment. You are fed lots of pizza, then more pizza and then you are asked to find your way across the city on a scooter powered only by pizza. Of course, the city has lots of intersections, and these intersections are very controlled. Some intersections are forbidden for you to enter; some only let you move north/south as you leave the intersection; others let you move only east/west as you leave the intersection; and the rest let you go in any compass direction (north, south, east or west).

Thankfully your scientific friends have given you a map of the city (on the back of a pizza box), with an arrangement of symbols indicating how you can move around the city. Specifically, there are 4 different symbols on the box:

- The symbol `+` indicates we can move in any direction (north/south/east/west) from this location.

- The symbol `-` indicates we can move only east or west from this location.

- The symbol `|` indicates we can move only north or south from this location.

- The symbol `*` indicates we cannot occupy this location.

Your task is to determine how many intersections you must pass through to move from the northwest corner of the city to the south-east corner of the city.

## 输入格式
The input begins with a number $t (1 \leq t \leq 10)$ on its own line, which indicates how many different cases are contained in this file. Each case begins with a number $r$ on one line, followed by a number $c$ on the next line $(1 \leq r, c \leq 20)$. The next $r$ lines contain $c$ characters, where each character is
one of {`+`, `*`, `-`, `|`}. You may assume the north-west corner of the city can be occupied (i.e., it will not be marked with `*`).

## 输出格式
The output will be $t$ lines long, with one integer per line. The integer on line $i (1 \leq i \leq t)$ indicates the minimum number of intersections required to pass through as you move from the north-west corner of the city to the south-east corner of the city. If there is no way to get from the north-west corner to the south-east corner, output $−1$ for that test case.

## 题目大意
一共有 $t(1 \leq t \leq 10)$ 组数据。

对于每组数据，给你一个 $r(1\leq r \leq 20)$ 行 $c(1\leq c \leq 20)$ 列的地图，你需要从地图的左上角，走到地图的右下角。

这个地图不是普通的地图，它并不是随随便便上下左右都能走的，你需要根据该格子上的字符，来对应其能走的方向：

- 为 `+`：上下左右都能走。

- 为 `-`：只能左右移动。

- 为 `|`：只能上下移动。

- 为 `*`：无法移动（不仅在该点无法往上下左右移动，而且甚至**无法到达该点**）。

请你判断它能不能从左上角走到右下角 （保证**左上**角不为 `*`），如果能，输出最小的步数，如果不能，输出 $-1$。

注：初始时在左上角和在右下角结束时都算 $1$ 步。 

```input1
3
2
2
-|
*+
3
5
+||*+
+++|+
**--+
2
3
+*+
+*+

```

```output1
3
7
-1
```

