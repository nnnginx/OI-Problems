## 题目描述

给定一个 $N$ 个顶点的凸多边形，求最大的 $R$ ，使得两个半径为 $R$ 的圆，在互不相交的情况下能被放入到这个多边形中。

## 输入格式

第一行一个整数 $N$ 。

接下来的 $N$ 行，每行两个空格分开的整数 $x_i , y_i$ ，表示凸多边形第 $i$ 个顶点的坐标。（保证顶点坐标按**逆时针**顺序给出）

## 输出格式

一个实数，表示最大的半径 $R$ 。

只要你的输出与标准答案的误差在 $10^{-3}$ 以内均被视为通过。

```input1
4
0 0
1 0
1 1
0 1
```

```output1
0.293
```

## 样例说明 1

将两个圆心放在该正方形的对角线上的时候，半径最长，如图：

![](https://hydro.org.cn/d/bzoj/p/2403/file/pic1.jpg)

此时半径为 $\frac{\sqrt{2}}{2\times(1+\sqrt{2})} \approx 0.293$ 。

```input2
4
0 0
3 0
3 1
0 1
```

```output2
0.500
```

```input3
6
0 0
8 0
8 6
4 8
2 8
0 4
```

```output3
6
0 0
8 0
8 6
4 8
2 8
0 4
```

## 数据规模与约定

对于 $10\%$ 的数据，保证 $N=3$ 。

对于 $40\%$ 的数据，保证 $N\le 250$ 。

对于 $100\%$ 的数据，保证 $3\le N \le 5\times 10^4 , -10^7 \le x_i,y_i \le 10^7$ 。

## 题目来源

[Balkan Olympiad in Informatics 2011](http://www.boi2011.ro/boi2011/) [Day 1](http://www.boi2011.ro/boi2011/?pagina=probleme) [T1 2circles](http://www.boi2011.ro/resurse/tasks/2circles.pdf)
