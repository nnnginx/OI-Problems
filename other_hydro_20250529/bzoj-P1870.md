## 题目描述

给出 $n$ 条直线，问他们将一个无限大平面分成了多少份，每一份的面积是多少。

## 输入格式

**本题有多组数据。**

The first line of the input file contains N �� the number of lines (1 <= N <= 80). Each of next N lines contains four integer numbers x1, y1, x2 and y2 - the coordinates of two different points of the line. All coordinates do not exceed 102 by their absolute value. No two lines coincide.

## 输出格式

First output K - the number of finite parts among those the lines divide the plane to. Next K lines of the output file must contain area parts sorted in non-decreasing order. You answer must be accurate up to 10-4. Due to floating point precision losses possible, do not consider parts with area not exceeding 10-8.

## 样例

```input1
1
5
0 0 1 0
1 0 1 1
1 1 0 1
0 1 0 0
0 0 1 1
```
```output1
2
0.5000
0.5000
```

## 数据规模与约定

对于 $100\%$ 的数据，保证 $1\le n\le 80,-102\le x_1,y_1,x_2,y_2\le 102$。

答案精确到 $4$ 位小数。

你不应该考虑面积小于 $10^{-8}$ 的多边形。

