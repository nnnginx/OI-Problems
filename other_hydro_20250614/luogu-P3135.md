## 题目描述
Bessie is building a fort with her friend Elsie. Like any good fort, this one needs to start with a sturdy frame. Bessie wants to build a frame in the shape of a one-meter-wide rectangular outline, atop which she will build the fort.

Bessie has already chosen a site on which to build the fort -- a piece of land measuring $N$ meters by $M$ meters ($1 \leq N, M \leq 200$). Unfortunately, the  site has some swampy areas that cannot be used to support the frame.  Please help Bessie determine the largest area she can cover with her fort (the area of the rectangle supported by the frame), such that the frame avoids sitting on any of the swampy areas.

## 输入格式
Line 1 contains integers $N$ and $M$.

The next $N$ lines each contain $M$ characters, forming a grid describing the site.  A character of '.' represents normal grass, while 'X' represents a swampy spot.

## 输出格式
A single integer representing the maximum area that Bessie can cover with her fort.

## 题目大意
### 题目描述

Bessie 正在和她的朋友 Elsie 一起建造一个堡垒。像任何好的堡垒一样，这个堡垒需要一个坚固的框架。Bessie 想要建造一个一米宽的矩形轮廓框架，然后在这个框架上建造堡垒。

Bessie 已经选择了一个建造堡垒的地点——一块 $N$ 米乘 $M$ 米的土地（$1 \leq N, M \leq 200$）。不幸的是，这块地有一些沼泽区域，不能用来支撑框架。请帮助 Bessie 确定她可以用堡垒覆盖的最大面积（由框架支撑的矩形的面积），使得框架不会坐落在任何沼泽区域上。

### 输入格式

第 1 行包含整数 $N$ 和 $M$。

接下来的 $N$ 行每行包含 $M$ 个字符，形成一个描述地点的网格。字符 '.' 表示普通草地，而 'X' 表示沼泽区域。

### 输出格式

一个整数，表示 Bessie 可以用堡垒覆盖的最大面积。

### 说明/提示

在示例中，最优框架的位置由下面的 `f` 表示：

```
.ffff.
.fX.fX
Xf.Xf.
.ffff.
..X...
```

```input1
5 6
......
..X..X
X..X..
......
..X...
```

```output1
16
```

## 提示
In the example, the placement of the optimal frame is indicated by 'f's below:

```cpp
.ffff.
.fX.fX
Xf.Xf.
.ffff.
..X...
```

