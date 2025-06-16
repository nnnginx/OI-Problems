## 题目描述

Art critics worldwide have only recently begun to recognize the creative genius behind the great bovine painter, Picowso.

Picowso paints in a very particular way. She starts with an $n \times n$ blank canvas, represented by an $n \times n$ grid of zeros, where a zero indicates an empty cell of the canvas. She then draws $n^2$ rectangles on the canvas, one in each of $n^2$ colors (conveniently numbered $1 \ldots n^2$). For example, she might start by painting a rectangle in color $2$, giving this intermediate canvas:

```
2 2 2 0

2 2 2 0

2 2 2 0

0 0 0 0
```

She might then paint a rectangle in color $7$:

```
2 2 2 0

2 7 7 7

2 7 7 7

0 0 0 0
```

And then she might paint a small rectangle in color $3$:

```
2 2 3 0

2 7 3 7

2 7 7 7

0 0 0 0
```

Each rectangle has sides parallel to the edges of the canvas, and a rectangle could be as large as the entire canvas or as small as a single cell. Each color from $1 \ldots n^2$ is used exactly once, although later colors might completely cover up some of the earlier colors.

Given the final state of the canvas, please count how many of the $n^2$ colors could have possibly been the first to be painted.

## 输入格式

The first line of input contains $n$, the size of the canvas.  
The next $n$ lines describe the final picture of the canvas, each containing $n$ integers that are in the range $0 \ldots n^2$. The input is guaranteed to have been drawn as described above, by painting successive rectangles in different colors.

## 输出格式

Please output a count of the number of colors that could have been drawn first.



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


## 说明

In this example, color $2$ could have been the first to be painted. Color $3$ clearly had to have been painted after color $7$, and color $7$ clearly had to have been painted after color $2$. Since we don&#039;t see the other colors, we deduce that they also could have been painted first.

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n\le 10^3$。

## 题目来源

Platinum