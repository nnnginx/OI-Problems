## 题目描述


Fiora is a game designer. Now she is designing the final level for her new game.

A level for this game is a labyrinth on a rectangular grid with lots of enemies. Player starts her game at the square $(0 , 0)$ and her purpose is to get to the square $(a , b)$ . Fiora has lots of ideas on how to put enemies, but she does not like designing labyrinths. She needs your help here.

Fiora is drawing levels in a special level editor which supports one basic block to design a labyrinth. This block is an L-shaped corner, consisting of two perpendicular rectangles $1 \times n$ squares in size intersecting at $1 \times 1$ square. It is possible to rotate this block in four ways. Blocks cannot intersect, but they can touch each other. Player can move through all the squares lying in any block. She can move between two squares if they are sharing a side, even if they are in different blocks.

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15288/1.png)

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15288/2.png)

![](https://onlinejudgeimages.s3-ap-northeast-1.amazonaws.com/problem/15288/3.png)

Blocks with $n = 3$

The first example

The second example

Fiora wants to design the final level with the minimal possible number of blocks. Of course, it should be possible to move from square $(0 , 0)$ to square $(a , b)$ .



## 输入格式


The first line of the input consists of a single integer $m (1 \le m \le 100)$ -- the number of test cases. It is followed by $m$ test cases. Each test case is on a separate line and consists of three integers a , $b$ , and $n (−10^{8} \le $ a , $b \le 10^{8}; 2 \le n \le 10^{8})$ -- a is the coordinate of the final point along the horizontal axis, $b$ is the coordinate of the final point along the vertical axis, and $n$ is the size of the block. The final point is not same as the starting one (either a $≠ 0$ or $b ≠ 0)$ .



## 输出格式


For each test case, in the first line print the minimal number $k$ of blocks you need. In the following $k$ lines print description of these blocks. Each L-shaped corner block is described by coordinates of two cells. Print coordinates of the end of its vertical rectangle, followed by coordinates of the end of its horizontal rectangle. Specify the coordinates of the ends that are opposite to the intersection of the rectangles. Note that the order of cells in the block description matters, since a change of the order results in a reflected block. Coordinates of each end should be printed with the coordinate along the horizontal axis first, followed by the coordinate along the vertical axis.

All coordinates in the output should not exceed $10^{9}$ by absolute value.

It is guaranteed that the total number of blocks in the correct output does not exceed $10^{5}$ for all test cases combined.



## 题目大意
用长度为 $n$ 的 L 型方块摆在二维网格平面上，仅通过方块从 $(0,0)$ 走到 $(a,b)$。

### 输入格式

第一行一个正整数 $m$ ，下面 $m$ 行每行 $3$ 个正整数 $a, b, n$。

### 输出格式

对于每组数据，输出最小 L 型块数 $k$，下面 $k$ 行每行按先横坐标后纵坐标的顺序输出每个 L 型块两端的坐标。

### 数据范围

对于 $100\%$ 的数据，$1 \le m \le 100, -10^8 \le a, b  \le 10^8, 2 \le n \le 10^8$。

```input1
2
2 3 2
4 -1 3

```

```output1
2
1 1 0 0
1 2 2 3
2
0 0 2 -2
3 -3 5 -1

```

## 提示
Time limit: 3 s, Memory limit: 512 MB. 



