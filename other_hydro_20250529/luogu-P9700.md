## 题目描述
$\textit{Peg Solitaire}$ is a single-player boardgame on a chessboard with $n$ rows and $m$ columns. Each cell of the chessboard either is empty, or contains a chesspiece. Initially, there are $k$ chesspieces on the chessboard.

During the game, the player can choose a chesspiece, jump it over an adjacent chesspiece into an empty cell, and finally remove the chesspiece which is jumped over. More precisely, let $(i, j)$ be the cell on the $i$-th row and the $j$-th column, the player can perform operations of the following four types.

![](https://cdn.luogu.com.cn/upload/image_hosting/ugauif68.png)

Given the initial state of the chessboard, the player can perform the operations any number of times (including zero times). Calculate the minimum possible number of chesspieces remaining on the chessboard.

## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$ ($1 \le T \le 20$) indicating the number of test cases. For each test case:

The first line contains three integers $n$, $m$ and $k$ ($1 \le n, m \le 6$, $1 \le k \le \min(6, n \times m)$) indicating the number of rows and columns of the chessboard and the initial number of chesspieces.

For the following $k$ lines, the $i$-th line contains two integers $x_i$ and $y_i$ ($1 \le x_i \le n$, $1 \le y_i \le m$) indicating that there is a chesspiece in the cell on the $x_i$-th row and the $y_i$-th column at the beginning. Except from these $k$ cells, all other cells are empty at the beginning. The positions of these $k$ cells contain no duplicate.

## 输出格式
For each test case output one line containing one integer indicating the minimum possible number of chesspieces remaining on the chessboard.


## 题目大意
**【题目描述】**

``独立钻石``是一种单人桌游。游戏在 $n$ 行 $m$ 列的棋盘上进行，棋盘上的每一格要么是空格，要么有一枚棋子。一开始，棋盘上共有 $k$ 枚棋子。

在游戏中，玩家可以选择一枚棋子，将它跳过相邻棋子到空格上，并移除被跳过的棋子。具体来说，令 $(i, j)$ 表示位于第 $i$ 行第 $j$ 列的格子，玩家可以执行以下四种操作。

![](https://cdn.luogu.com.cn/upload/image_hosting/pgosoztu.png)

给定一个初始的棋盘，求经过任意次操作（包括零次）之后，棋盘上最少能剩余几枚棋子。

**【输入格式】**

有多组测试数据。第一行输入一个整数 $T$（$1 \le T \le 20$）表示测试数据组数。对于每组测试数据：

第一行输入三个整数 $n$，$m$ 和 $k$（$1 \le n, m \le 6$，$1 \le k \le \min(6, n \times m)$）表示棋盘的行数，列数和初始棋子的数量。

对于接下来 $k$ 行，第 $i$ 行输入两个整数 $x_i$ 和 $y_i$（$1 \le x_i \le n$，$1 \le y_i \le m$）表示一开始第 $x_i$ 行第 $y_i$ 列的格子里有一枚棋子。除了这 $k$ 个格子之外，其它格子一开始都是空格。这 $k$ 个格子的位置不会重复。

**【输出格式】**

每组数据输出一行一个整数，表示经过任意次操作（包括零次）之后，棋盘上最少能剩余几枚棋子。

**【样例解释】**

第一组样例数据解释如下。

![](https://cdn.luogu.com.cn/upload/image_hosting/aragowha.png)

对于第二组样例数据，由于初始棋盘不存在空格，因此无法进行任何操作。

对于第三组样例数据，由于棋盘不足三格，因此无法进行任何操作。

```input1
3
3 4 5
2 2
1 2
1 4
3 4
1 1
1 3 3
1 1
1 2
1 3
2 1 1
2 1
```

```output1
2
3
1
```

## 提示
The first sample test case is explained as follows.

![](https://cdn.luogu.com.cn/upload/image_hosting/aragowha.png)

For the second sample test case, as the chessboard does not contain empty cell at the beginning, the player cannot perform any operation.

For the third sample test case, as the chessboard has less than three cells, the player cannot perform any operation.


