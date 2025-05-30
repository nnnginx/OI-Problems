## 题目描述


Last month, Sichuan province secured funding to establish the Great Panda National Park, a natural preserve for a population of more than $1 800$ giant pandas. The park will be surrounded by a polygonal fence. In order for researchers to track the pandas, wireless receivers will be placed at each vertex of the enclosing polygon and each animal will be outfitted with a wireless transmitter. Each wireless receiver will cover a circular area centered at the location of the receiver, and all receivers will have the same range. Naturally, receivers with smaller range are cheaper, so your goal is to determine the smallest possible range that suffices to cover the entire park.

As an example, Figure G.1 shows the park described by the first sample input. Notice that a wireless range of $35$ does not suffice (a) , while the optimal range of $50$ covers the entire park (b) .

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15695/1.png)

Figure G.1 : Illustration of Sample Input $1$ .



## 输入格式


The first line of the input contains an integer $n (3 \le n \le 2 000)$ specifying the number of vertices of the polygon bounding the park. This is followed by $n$ lines, each containing two integers $x$ and $y (|x|, |y| \le 10^{4})$ that give the coordinates $(x , y)$ of the vertices of the polygon in counter-clockwise order. The polygon is simple; that is, its vertices are distinct and no two edges of the polygon intersect or touch, except that consecutive edges touch at their common vertex.



## 输出格式


Display the minimum wireless range that suffices to cover the park, with an absolute or relative error of at most $10^{−6}.$



## 题目大意
给定一个 $n$ 个点的不自交的多边形（不一定是凸多边形），求最小的圆半径 $r$ 使得在每个顶点画一个半径为 $r$ 的圆，这些圆的并覆盖了整个多边形。$n \le 2000$，绝对误差或相对误差不超过 $10^{-6}$。

```input1
5
0 0
170 0
140 30
60 30
0 70

```

```output1
50

```

```input2
5
0 0
170 0
140 30
60 30
0 100

```

```output2
51.538820320

```

```input3
5
0 0
1 2
1 5
0 2
0 1

```

```output3
1.581138830

```

## 提示
Time limit: 10 s, Memory limit: 1024 MB. 



