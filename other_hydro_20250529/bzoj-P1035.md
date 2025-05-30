## 题目描述

经过连续若干年的推广，Risk 这个游戏已经风靡全国，成为大众喜闻乐见的重要娱乐方式。Risk 这个游戏可以理解为一种简易的策略游戏，游戏者的目的是占领所有的土地。由于游戏规则的规定，只要两个国家相邻，就认为两个国家有交战的可能性。我们现在希望知道在当前的局面下，哪些国家之间有交战的可能性。注意，我们认为只有当两个国家的国界线有公共边的时候才认为相邻，若两个国家的领土只有公共点，则认为两个国家不相邻。

![pic1.jpg](./585/file/pic1.jpg)

每一个国家的边界由一系列线段组成，保证这个边界是一个简单多边形，即严格不自交。为了定位每个国家的位置，我们还给出每个国家最庞大的一支军队的位置，保证这个位置一定出现在某一个形内，而不是出现在某条边界上。

## 输入格式

输入文件的第一行中包括两个整数 $n,m$。分别表示地图上的国家数和描述国家的边界的线段的数量。接下来 $n$ 行，每行用一对数描述了某个国家的主力军队的坐标。接下来m行，每行有 $4$ 个数 $x1,y1,x2,y2$，$(x1,y1)\sim(x2,y2)$ 描述了一条国界线。所有点的坐标都是 $0\sim 10^4$ 之间的整数。

保证输入的所有线段至多只会在线段交点处相交。整张地图上有且仅有一块面积无限的空白区域不属于任何国家。每一条国界线两侧的区域或者隶属于两个不同的国家，或者分隔了一个国家与那块无穷大的空白区域。即保证一条国界线两侧的区域不同时属于同一个国家或是同时都是空白区域。所有封闭区域内部包含且仅包含一支主力军队，表示了该区域的归属。

![pic1.jpg](./585/file/pic1.jpg)

例如上图中第一行的数据是合法的。而第二行中的数据都是不合法的。左边的那幅图包含线段两侧都是空白区域；中间的图包含线段两侧区域同时属于同一个国家；右边的图中军队被布置在了国界线上，因此非法；此外若最右侧的图中若没有军队也是非法的。保证输入文件提供的数据都是合法的，你的程序不需要进行数据合法性的判定。

## 输出格式

输出文件包括 $n$ 行，每行第一个数字 $x$ 表示有 $x$ 个国家可能与这个国家交战，接着在同一行中升序输出 $x$ 个整数，表示可能与这个国家交战的国家的编号。国家按输入中给出的顺序从 $1$ 到 $n$ 编号。注意数字间严格以一个空格隔开，并且不要在行末输出多余的空白字符。


```input1
4 12
3 2
11 8
12 17
1 19
0 0 10 0
10 0 20 0
20 0 20 10
20 10 20 20
20 20 10 20
10 20 0 20
0 20 0 10
0 10 0 0
10 0 10 10
0 10 10 10
20 10 10 10
10 20 10 10
```


```output1
2 2 4
2 1 3
2 2 4
2 1 3
```


```input2
4 16
170 13
24 88
152 49
110 130
60 60 140 60
140 60 140 140
140 140 60 140
60 140 60 60
0 0 200 0
200 0 200 200
200 200 0 200
0 200 0 0
40 40 160 40
160 40 160 160
160 160 40 160
40 160 40 40
20 20 180 20
180 20 180 180
180 180 20 180
20 180 20 20
```


```output2
1 2
2 1 3
2 2 4
1 3
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n\le 600$，$1\le m\le 4\times 10^3$。
