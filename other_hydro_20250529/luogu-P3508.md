## 题目描述
In the middle of the night Bitratio turned on the lamp at the entrance to the building that Byteasar lives in.

Now the strong light prevents Byteasar from sleeping.

While the lamp does not shine directly on Byteasar's windows, it does so by reflecting in other windows.

Deprived of sleep, Byteasar is becoming irritated.

To remedy that he tries to occupy his mind, but all he can think of is the light.

Thus Byteasar looked out the window and wondered if his neighbours suffer similar torture,    i.e., whether the light shines on their windows as well.

Now that is an interesting question, at least in Byteasar's opinion.

You learn of the puzzle sooner than you would wish: unable to solve the problem all by himself,    thinking little of sleep now (be it his and yours), Byteasar calls you to ask for help.

You know him well enough to understand that you too will not get any sleep until you write a program    that solves his problem.

Byteasar lives in the building ![](http://main.edu.pl/images/OI17/lat-en-tex.1.png), which has ![](http://main.edu.pl/images/OI17/lat-en-tex.2.png) windows.

The lamp is situated on a wall at the very bottom of this building.

Opposite the building ![](http://main.edu.pl/images/OI17/lat-en-tex.3.png), exactly 10 meters apart, there is another building, ![](http://main.edu.pl/images/OI17/lat-en-tex.4.png).

The wall of this ![](http://main.edu.pl/images/OI17/lat-en-tex.5.png)-windowed building is parallel to the wall of ![](http://main.edu.pl/images/OI17/lat-en-tex.6.png), the Byteasar's building.

The lamp light behaves like you would expect, i.e., in the way predicted by geometrical optics (or ray optics).

Namely the light propagates along rays, and if a ray hits a window, it is reflected.

Due to The Law of Reflection, the angle of the ray's reflection equals the angle of incidence.

We introduce coordinate systems on the the walls of the two buildings in the following way.

Both ![](http://main.edu.pl/images/OI17/lat-en-tex.7.png) axes are horizontal, while both ![](http://main.edu.pl/images/OI17/lat-en-tex.8.png) axes are vertical; the axes on both walls are identically oriented,    and the ![](http://main.edu.pl/images/OI17/lat-en-tex.9.png) points of the walls are opposite one another.

The windows (on either building) are simply rectangles with sides parallel to the axes of the coordinate system.

A ray is reflected only in the interior of any window; it is absorbed on the window's boundary.

In each building, no two windows share any part of their interiors.

The lamp is located on the wall of the ![](http://main.edu.pl/images/OI17/lat-en-tex.10.png) building at the point ![](http://main.edu.pl/images/OI17/lat-en-tex.11.png),    which is neither inside nor at the boundary of any window.


## 输入格式
In the first line of the standard input there are two integers ![](http://main.edu.pl/images/OI17/lat-en-tex.12.png) and ![](http://main.edu.pl/images/OI17/lat-en-tex.13.png) (![](http://main.edu.pl/images/OI17/lat-en-tex.14.png)),      separated by a single space, denoting the number of windows in the first and second building respectively.

The ![](http://main.edu.pl/images/OI17/lat-en-tex.15.png) lines that follow describe the windows in Byteasar's building (the ![](http://main.edu.pl/images/OI17/lat-en-tex.16.png) building), one per line.

The line no. ![](http://main.edu.pl/images/OI17/lat-en-tex.17.png) (for ![](http://main.edu.pl/images/OI17/lat-en-tex.18.png)) holds four integers ![](http://main.edu.pl/images/OI17/lat-en-tex.19.png), ![](http://main.edu.pl/images/OI17/lat-en-tex.20.png), ![](http://main.edu.pl/images/OI17/lat-en-tex.21.png), ![](http://main.edu.pl/images/OI17/lat-en-tex.22.png)      (![](http://main.edu.pl/images/OI17/lat-en-tex.23.png),      !…


## 输出格式
In the first line of the standard output your program should print the number of windows in the ![](http://main.edu.pl/images/OI17/lat-en-tex.31.png) building      whose interiors are hit by some ray.

You may assume that in every test instance there will be at least one such window (the Byteasar's window).

In the second line the numbers of these windows (windows are numbered starting from 1) should be printed in increasing order,      separated by single spaces.


## 题目大意
一天，~~**缺德的**~~ Bitratio 打开了 Byteasar 所居住的大楼处的灯光。

Byteasar 无法入睡的时候，~~**缺德的**~~ 他开始想知道他的邻居是否也遭受了类似的折磨，也就是说，光线是否也照在他们的窗户上。

已知这个世界归牛顿管理。也就是说，光沿着光线传播，如果光线击中窗口，就会被反射。且根据反射定律，光线的反射角等于入射角。

~~**缺德的**~~ Bitratio 所住的大楼与 Byteasar 的大楼相距 $10m$ 。它们的墙壁都是平行的，光线只在任何窗户的内部反射，反之，它在窗口的边界上被吸收。

我们以以下方式在这两栋建筑的墙上引入坐标系：两个轴都是水平的，而两个轴是垂直的；两个墙上的轴线方向相同，墙的点彼此相对。窗户（在任何一栋建筑上）都是简单的矩形，侧面平行于坐标系的轴。在每栋建筑中，没有两扇窗户共享其内部的任何部分。该灯位于建筑物的墙上，该点既不在任何窗户的内部，也不在任何窗口的边界。

## 输入输出格式

**输入部分**：第一行为两个整数 $n$ , $m$ ，分别表示第一栋和第二栋建筑中的窗户数量。之后 $n+m$ 行，描述了 Byteasar 与 Bitratio 的大楼中窗户的位置。每行包含四个整数 $x_1$ , $y_1$ , $x_2$ , $y_2$ ，表示窗户左上角和右下角的坐标。

**输出部分**：两行，第一行表示 Byteasar 的大楼中被照射到的窗户的数量 $k$ ，第二行输出 $k$ 个整数，表示被照射到的窗户的编号。

```input1
3 3
-1 2 1 4
-1 5 1 7
-3 8 -2 20
-1 1 1 2
-1 4 1 5
-1 7 1 10
```

```output1
2
1 2
```

## 提示
$-1000 \le x_{1,i} \lt x_{2,i} \le 1000$，$0 \le y_{1,i} < y_{2,i} \le 1000$


