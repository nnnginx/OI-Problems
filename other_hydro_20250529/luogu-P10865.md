## 题目描述
Blue-edged Shot is forbidden from playing Genshin Impact by LeavingZ. However, today LeavingZ went to Huazhong University of Science and Technology, School of Cyber Science and Engineering, to harvest the gold medal of the 2024 International Collegiate Programming Contest in Hubei Province, China.

An activity of Genshin Impact called `Dodoco's Bomb-Tastic Adventure` has begun. This is a single-player game, where each game involves a pond. The pond can be divided into an $n$ by $m$ grid, with the cell in the $i$-th row and $j$-th column represented by $(i,j)$. Among these, $k$ cells contain fish, and you will play as the Spark Knight Klee, who fishes with explosives.

![](https://cdn.luogu.com.cn/upload/image_hosting/3keap2xe.png)

If Klee drops a bomb at $(a,b)$, all the cells $(x,y)$ satisfying $|x-a|+|y-b|\le 1$ will be covered by the explosion. For every cell covered by the explosion, Klee will catch one fish from it. Klee can drop bombs at any location. The question is, to catch all the fish, how many `Jumpy Dumpty` bombs are needed at a minimum?

## 输入格式
The first line contains three integers $n,m,k$ ($1 \le n,m \le 10^3, 1 \le k \le 10$) --- the size of the grid and the number of cells containing fish.

The following $k$ lines, each line contains three integers $x_i,y_i,a_i$ ($1\le x_i \le n, 1 \le y_i \le m, 1 \le a_i \le 3$), representing there are $a_i$ fish in cell $(x_i,y_i)$.

It is guaranteed that the input cell $(x_i,y_i)$ are unique.

## 输出格式
Output a single integer, denoting the minimum number of bombs needed.

## 题目大意
### 题目描述
“Blue-edged Shot 被 LeavingZ 禁止玩《原神》。然而，今天 LeavingZ 前往了华中科技大学的网络科学与工程学院，参加2024年中国湖北省国际大学生程序设计竞赛，并收获了金牌。

《原神》中的一个活动多多炸弹大冒险已经开始了。这是一个单人游戏，每局游戏都涉及一个池塘。池塘可以被划分为一个 $n×m$ 的网格，其中第 $i$ 行第 $j$ 列的单元格表示为 $(i,j)$。在这些单元格中，有 $k$ 个单元格包含鱼，你将扮演火花骑士克莱，她用炸药来捕鱼。

如果克莱在 $(a,b)$ 位置投放炸弹，那么所有满足$|x-a|+|y-b|\le 1$的单元格 $(x,y)$ 都将被爆炸覆盖。对于每一个被爆炸覆盖的单元格，克莱都会从其中捕到一条鱼。克莱可以在任何位置投放炸弹。问题是，为了捕到所有的鱼，至少需要多少枚`蹦蹦炸弹`？”
### 输入格式
第一行包含三个整数 $n,m,k$ ($1 \le n,m \le 10^3, 1 \le k \le 10$)，分别表示网格的大小（行数和列数）以及包含鱼的单元格数量。

接下来的 $k$ 行，每行包含三个整数 $x_i,y_i,a_i$ ($1\le x_i \le n, 1 \le y_i \le m, 1 \le a_i \le 3$)，表示在网格的 ($x_i, y_i$) 单元格中有 $a_i$ 条鱼。

输入保证所有的 $(x_i, y_i)$ 单元格坐标都是唯一的。
### 输出格式
输出一个整数，表示所需的最少炸弹数量。” 在这个问题中，你需要计算并输出一个整数，该整数代表为了捕获所有鱼所需投放的最少“蹦蹦炸弹”数量。
### 样例 #1

#### 样例输入 #1

```
5 5 3
1 1 2
2 2 1
5 5 2
```

#### 样例输出 #1

```
4
```
### 提示

一种可能的方法是在 $(1,2)$ 位置投放两枚炸弹，再在 $(5,5)$ 位置投放另外两枚炸弹。

可以证明没有比这个答案更小的解。

```input1
5 5 3
1 1 2
2 2 1
5 5 2
```

```output1
4
```

## 提示
One possible way is to drop two bombs at $(1,2)$ and another two at $(5,5)$.

It can be proven that there is no solution with a smaller answer.

