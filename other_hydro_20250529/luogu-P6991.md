## 题目背景
这是一道 IO 交互题。

## 题目描述


This is an interactive problem.

Gomoku is a two-player game on a two-dimensional grid. Each cell of the grid can be either empty, contain the first player's mark $(black),$ or contain the second player's mark $(white),$ but not both. Initially the entire grid is empty. Two players make alternating moves, starting with the first player. At each move, a player can put her mark into exactly one empty cell. The first player to have her five adjacent marks in a single row wins. The winning row can be either vertical, horizontal or diagonal.

![](https://upload.acmicpc.net/23c94254-2783-405a-907b-7b66bea5514b/-/preview/)

Position where the second player (white marks) had won.

The players use a $19 \times 19$ grid in this problem. If the entire grid gets filled with marks but no player has won, the game is declared a draw.

The first player uses the following strategy: as the first move, she puts her mark into the center cell of the grid. At every other move, she picks such a move that maximizes the score of the resulting position.

In order to find the score of a position, the first player considers all possible places where the winning combination might eventually form -- in other words, all horizonal, vertical and diagonal rows of five consecutive cells on the board (of course, they may overlap each other). If such a row contains both the first player's marks and the second player's marks, it is disregarded. If such a row contains no marks, it is disregarded as well. For each row with exactly $k (1 \le k \le 5)$ marks of the first player and no marks of the second player, add $50^{2k−1}$ to the score of the position. For each row with exactly $k$ marks of the second player and no marks of the first player, subtract $50^{2k}$ from the score of the position. Finally, add a random integer number between $0$ and $50^{2} − 1$ to the score. This random number is chosen uniformly.

In case when several moves of the first player have equal scores (such ties are quite rare because of the random addition mentioned above), the first player picks the one with the smallest x-coordinate, and in case of equal x-coordinates, the one with the smallest y-coordinate.

Your task is to write a program that plays the second player and beats this strategy.

Your program will play $100$ games against the strategy described above, with different seeds of random generator. Your program must win all these games.



## 题目大意
这是一道交互题。

五子棋是一种两个人在二维棋盘上玩的游戏。棋盘上的每个格子可以为空，放有第一名玩家的棋子（黑），或者放有第二名玩家的棋子（白），但是不能都有。初始时所有的格子都是空的。两个玩家轮流操作，从第一名玩家开始。每次操作，一名玩家可以把他的棋子放进恰好一个空格子里。首先在一行中放下五个相邻棋子的玩家获胜。一行可以是横行、竖行或对角线。

![1.png](https://upload.acmicpc.net/23c94254-2783-405a-907b-7b66bea5514b/-/preview/)

*第二名玩家（白子）获胜的一种情况。*

在这个问题中，玩家们使用 $19 \times 19$ 的棋盘。如果整个棋盘都放满了棋子但无人获胜，游戏平局。

第一名玩家将会使用下面的策略：第一次操作时，她会把她的棋子放到棋盘的正中间。在后面的每次操作中，她会选择一个下子后局面分数最大的位置下子。

为了计算一个局面的分数，第一名玩家会考虑能组成胜利组合的所有地方——换句话说，棋盘上所有横行、竖行、对角线上五个连续的格子（当然，它们会互相重叠）。如果这一行同时包括了第一名玩家的棋子和第二名玩家的棋子，就无视它。如果这一行包括了恰好 $k\ (1\le k\le 5)$ 个第一名玩家的棋子而没有第二名玩家的棋子，给该局面的分数加上 $50^{2k-1}$。如果这一行包括了恰好 $k$ 个第二名玩家的棋子而没有第一名玩家的棋子，给该局面的分数减去 $50^{2k}$。最后，给分数加上一个 $0$ 到 $50^2-1$ 的随机数。随机数是均匀分布的。

如果第一名玩家有多个分数相同的格子可选（因为上面提到的随机分数的原因，这是非常罕见的），第一名玩家选择 X 坐标最小的位置，如果仍有多个格子有相同的 X 坐标，就选择 Y 坐标最小的位置。

你的任务是，写一个程序扮演第二名玩家，并打败上述的策略。

你的程序将会与上述策略对局 $100$ 局，每局的随机数种子不同。你的程序必须在每局中都获胜。

### 交互格式

每一步你的程序需要做：

1. 从标准输入读入两个整数 $x,y$。
2. 如果都是 $-1$，那么游戏结束，你的程序必须退出。
3. 否则这两个整数描述了第一名玩家下子的坐标，$1\le x,y\le 19$。
4. 输出第二名玩家下子的坐标，然后换行。别忘了清空缓冲区。

### 样例

在下面的样例中，第一名玩家**没有**使用题目描述中所述的策略。这个样例只是为了说明交互格式。

![2.png](https://s1.ax1x.com/2020/10/29/B8voct.png)

*样例最终的棋盘状态。*

### 说明

世界上有很多种不同的五子棋规则。请只考虑题目描述中说明的这一种规则。

```input1
10 10
10 11
10 12
10 13
9 10
9 11
9 9
11 13
-1 -1

```

```output1
11 10
11 11
10 9
10 14
8 9
11 9
11 12
11 8

```

## 提示
Time limit: 2 s, Memory limit: 512 MB. 



