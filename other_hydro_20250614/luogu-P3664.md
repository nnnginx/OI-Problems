## 题目描述
Art critics worldwide have only recently begun to recognize the creative genius behind the great bovine painter, Picowso.


Picowso paints in a very particular way. She starts with an $N \times N$ blank canvas, represented by an $N \times N$ grid of zeros, where a zero indicates an empty cell of the canvas. She then draws $N^2$ rectangles on the canvas, one in each of $N^2$ colors (conveniently numbered $1 \ldots N^2$). For example, she might start by painting a rectangle in color 2, giving this intermediate canvas:


```
2 2 2 0

2 2 2 0

2 2 2 0

0 0 0 0
```




She might then paint a rectangle in color 7:

```
2 2 2 0

2 7 7 7

2 7 7 7

0 0 0 0
```




And then she might paint a small rectangle in color 3:

```
2 2 3 0

2 7 3 7

2 7 7 7

0 0 0 0
```


Each rectangle has sides parallel to the edges of the canvas, and a rectangle could be as large as the entire canvas or as small as a single cell. Each color from $1 \ldots N^2$ is used exactly once, although later colors might completely cover up some of the earlier colors.


Given the final state of the canvas, please count how many of the $N^2$ colors could have possibly been the first to be painted.

## 输入格式
The first line of input contains $N$, the size of the canvas ($1 \leq N \leq 1000$).

The next $N$ lines describe the final picture of the canvas, each containing $N$ integers that are in the range $0 \ldots N^2$. The input is guaranteed to have been drawn as described above, by painting successive rectangles in different colors.


## 输出格式
Please output a count of the number of colors that could have been drawn first.


## 题目大意
### 题目描述

世界各地的艺术评论家最近才开始认识到伟大的奶牛画家 Picowso 的创作天才。

Picowso 以一种非常独特的方式作画。她从一个 $N \times N$ 的空白画布开始，画布用一个 $N \times N$ 的零网格表示，其中零表示画布的一个空单元格。然后她在画布上绘制 $N^2$ 个矩形，每个矩形使用 $N^2$ 种颜色中的一种（方便地用编号 $1 \ldots N^2$ 标识）。例如，她可能首先用颜色 2 绘制一个矩形，得到以下中间画布：

```
2 2 2 0

2 2 2 0

2 2 2 0

0 0 0 0
```

然后她可能用颜色 7 绘制一个矩形：

```
2 2 2 0

2 7 7 7

2 7 7 7

0 0 0 0
```

接着她可能用颜色 3 绘制一个小矩形：

```
2 2 3 0

2 7 3 7

2 7 7 7

0 0 0 0
```

每个矩形的边都与画布的边缘平行，矩形可以大到整个画布，也可以小到一个单元格。每种颜色从 $1 \ldots N^2$ 恰好使用一次，尽管后来的颜色可能会完全覆盖一些先前的颜色。

给定画布的最终状态，请计算有多少种颜色可能是第一个被绘制的。

### 输入格式

输入的第一行包含 $N$，表示画布的大小（$1 \leq N \leq 1000$）。

接下来的 $N$ 行描述画布的最终状态，每行包含 $N$ 个整数，范围在 $0 \ldots N^2$。输入保证是按照上述方式通过连续绘制不同颜色的矩形生成的。

### 输出格式

请输出可能是第一个被绘制的颜色的数量。

### 说明/提示

在这个例子中，颜色 2 可能是第一个被绘制的。颜色 3 显然必须在颜色 7 之后绘制，而颜色 7 显然必须在颜色 2 之后绘制。由于我们没有看到其他颜色，我们推断它们也可能是第一个被绘制的。

```input1
4
2 2 3 0
2 7 3 7
2 7 7 7
0 0 0 0
```

```output1
14
```

## 提示
In this example, color 2 could have been the first to be painted. Color 3 clearly had to have been painted after color 7, and color 7 clearly had to have been painted after color 2. Since we don't see the other colors, we deduce that they also could have been painted first.

