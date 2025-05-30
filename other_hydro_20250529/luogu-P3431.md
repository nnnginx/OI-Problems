## 题目描述
The streets of Byte City form a regular, chessboardlike network - they are either north-south or west-east directed. We shall call them NS- and WE-streets. Furthermore, each street crosses the whole city. Every NS-street intersects every WE- one and vice versa. The NS-streets are numbered from $1$ to $n$, starting from the westernmost. The WE-streets are numbered from $1$ to $m$, beginning with the southernmost. Each intersection of the $i$'th NS-street with the $j$'th WE-street is denoted by a pair of numbers $(i,j)$ (for $1\le i\le n$, $1\le j\le m$).

There is a bus line in Byte City, with intersections serving as bus stops. The bus begins its itinerary by the $(1,1)$ intersection, and finishes by the $(n,m)$ intersection. Moreover, the bus may only travel in the eastern and/or northern direction.

There are passengers awaiting the bus by some of the intersections. The bus driver wants to choose his route in a way that allows him to take as many of them as possible. (We shall make an assumption that the interior of the bus is spacious enough to take all of the awaiting passengers, regardless of the route chosen.)TaskWrite a programme which:

reads from the standard input a description of the road network and the number of passengers waiting at each intersection,finds, how many passengers the bus can take at the most,writes the outcome to the standard output.


## 输入格式
The first line of the standard input contains three positive integers $n$, $m$ and $k$ - denoting the number of NS-streets, the number of WE-streets and the number of intersections by which the passengers await the bus, respectively ($1\le n\le 10^9$, $1\le m\le 10^9$, $1\le k\le 10^5$).

The following $k$ lines describe the deployment of passengers awaiting the bus, a single line per intersection. In the $(i+1)$'st line there are three positive integers $x_i$, $y_i$ and $p_i$, separated by single spaces, $1\le x_i\le n$,$1\le y_i\le m$,$1\le p_i\le 10^6$ . A triplet of this form signifies that by the intersection$(x_i,y_i)p_i$ passengers await the bus. Each intersection is described in the input data once at the most. The total number of passengers waiting for the bus does not exceed $1\ 000\ 000\ 000$.


## 输出格式
Your programme should write to the standard output one line containing a single integer - the greatest number of passengers the bus can take.


## 题目大意
Byte City 的街道形成了一个标准的棋盘网络，他们要么是北南走向要么就是西东走向。北南走向的路口从 $1$ 到 $n$ 编号, 西东走向的路从 $1$ 到 $m$ 编号。 每个路口用两个数 $(i,j)$ 表示 $(1 \le i \le n, 1 \le j \le m)$。 Byte City 里有一条公交线, 在某一些路口设置了公交站点。 公交车从 $(1, 1)$ 发车, 在 $(n, m)$ 结束。公交车只能往北或往东走。 现在有一些乘客在某些站点等车。 公交车司机希望在路线中能接到尽量多的乘客。帮他想想怎么才能接到最多的乘客。

```input1
8 7 11
4 3 4
6 2 4
2 3 2
5 6 1
2 5 2
1 5 5
2 1 1
3 1 1
7 7 1
7 4 2
8 6 2
```

```output1
11
```

