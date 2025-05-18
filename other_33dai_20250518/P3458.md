## 题目描述
Vicomte de Bajteaux is the owner of a renowned collection of boulders. Up to now, he has kept it in thecellars of his palace, but recently, he has decided to display the collection in his vast gardens.

The gardens have a shape of rectangle, whose sides are $1\ 000\ 000\ 000$ units long and are parallel to east-westand north-south geographical directions. For each boulder, vicomte has determined coordinates ofthe point, which he would like it to be placed in (the coordinates are simply distances to the southern and    western side of the garden), and gave them to his servants. Unfortunately he has forgot to tell them the orderof the coordinates (i.e. for some of the boulders the first coordinate of a point is the so called "$y$ coordinate",i.e. the ordinate, while for others the so called "$x$ coordinate", i.e. the abscissa).

The servants, unaware of thisfact, have placed the boulders assuming customary coordinate ordering (as in standard Cartesian coordinates:

the abscissa, commonly known as "$x$ coordinate", first).

To protect his collection, vicomte has decided to surround it with a fence. For aesthetic reasons thefence has to be a rectangle, with sides parallel to the sides of the garden. The garden layout has been planned,      so that the total length of the fence be minimal (i.e. in the space of all coordinate orderings, the original          ordering of vicomte requires the minimal length of the fence - we assume that the rectangle may have sides of zero length).

The servants have to move the boulders so that the length of the fence required is minimal lest their mistake become obvious. Each boulder may only be moved in a way that preserves the coordinate set: by      interchanging its coordinates. As the boulders are heavy, the servants would like to minimize their effort, by      minimizing the weight of the boulders to be moved.

## Task

Write a programme which:

reads the present positions of the boulders in the gardens and their respective weights, determines a sequence of moves, which minimizes the length of the fence required to protect the    boulders and also minimizes the weight of the boulders to be moved, writes the outcome to the standard output.

## 输入格式
The first line of the standard input contains a single integer $n$ ($2 \le n \le 1\ 000\ 000$), denoting the number of boulders in the collection. The following $n$  lines contain three integers $x_i$, $y_i$ and $m_i$ each ($0 \le x_i, y_i \le 1\ 000\ 000\ 000$, $1 \le m \le 2000$), separated by single spaces, denoting the present coordinates and the weight of $i$'th boulder. No unordered pair of coordinates will appear in the input more than once.


## 输出格式
The first line of the standard output should contain two integers, separated by a single space - the minimal length of fence possible and the minimal weight of the boulders to be moved in order to obtain such a length.


The second line should contain a sequence of $n$ zeros and/or ones - $i$'th element of the sequence should be a one if in the optimal solution the $i$'th boulder is to be moved and zero otherwise. Should more than one correct solutions exist, your programme is to write out any one of them.


## 题目大意
### 题目描述

**译自 POI 2007 Stage 2. Day 1「[Skalniak](https://szkopul.edu.pl/problemset/problem/s5ECsFKlMHti0g29uVkdKlQw/site/?key=statement)」**

Vicomte de Bajteaux 收藏了许多石头并准备把它们放到花园里。

花园是一个正方形，边长为 $1\ 000\ 000\ 000$。Vicomte de Bajteaux 让他的仆人为他用石头布置花园。但他忘记告诉仆人坐标的顺序，以至于一些点的坐标以 $(x,y)$ 的形式给出，一些点的坐标以 $(y,x)$ 的形式给出，并且石头已经按这样的顺序放好了。

为了保护石头，Vicomte de Bajteaux 按照实际的坐标规划了一排栅栏来围住这些石头，使得栅栏的总长最小。为了美观，栅栏必须是平行于坐标轴的矩形。为了让错误不那么明显，你需要帮助仆人选择一部分石头并将它们从 $(x,y)$ 移动到 $(y,x)$，在最小化栅栏的长度的基础上最小化需要移动的石头的总重。

### 输入格式

第一行一个整数 $n (1 \le n \le 1\ 000\ 000)$，表示石头的个数。

接下来 $n$ 行每行三个整数 $x_i, y_i, m_i$（$0 \le x_i,y_i \le 1\ 000\ 000\ 000, 1 \le m_i \le 2\ 000$），表示石头当前所在的坐标和重量。

不会有 $x$ 和 $y$ 组成的无序数对出现超过一次。

### 输出格式

第一行输出两个整数，分别表示栅栏的最小长度和需要移动的石头总重量的最小值。

第二行输出一个长度为 $n$ 的 01 串，表示取到石头总重量最小值的一种移动方案。第 $i$ 个字符为 $1$ 表示需要将第 $i$ 个石头从 $(x_i, y_i)$ 移动到 $(y_i, x_i)$，为 $0$ 则表示不需要。若有多解，输出任意一种解法均可以。

### 样例解释

![](https://cdn.luogu.com.cn/upload/image_hosting/gjo0jemf.png)

![](https://cdn.luogu.com.cn/upload/image_hosting/09zdeg0c.png)

翻译来自于 [LibreOJ](https://loj.ac/p/2655)。

```input1
5
2 3 400
1 4 100
2 2 655
3 4 100
5 3 277
```

```output1
10 200
01010
```

