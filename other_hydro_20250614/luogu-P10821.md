## ��Ŀ����
Prof. Pang plays chess against his rival Prof. Shou. They are the only two players in the game. The chessboard is very large and can be viewed as a 2D plane. Prof. Pang placed $n_1$ rooks and Prof. Shou placed $n_2$ rooks. Each rook is a point with integer coordinates on the chessboard. One rook is $\textit{attacked}$ by another rook if they satisfy all of the following conditions:

- They are placed by different players.
- They have the same $x$-coordinate or $y$-coordinate.
- There is no other rook on the line segment between them.

Help Prof. Pang and Prof. Shou to decide which rooks are attacked.

## �����ʽ
The first line contains two integers $n_1, n_2$ ($1\le n_1, n_2\le 200000$) separated by a single space denoting the number of rooks placed by Prof. Pang and the number of rooks placed by Prof. Shou.

The $i$-th ($1\le i\le n_1$) line of the next $n_1$ lines contains two integers $x, y$ ($-10^9\le x, y\le 10^9$) separated by a single space denoting the location $(x, y)$ of the $i$-th rook placed by Prof. Pang.

The $i$-th ($1\le i\le n_2$) line of the next $n_2$ lines contains two integers $x, y$ ($-10^9\le x, y\le 10^9$) separated by a single space denoting the location $(x, y)$ of the $i$-th rook placed by Prof. Shou.

It is guaranteed that the $n_1+n_2$ rooks placed by the players are distinct (i.e., no two rooks can have the same location).

## �����ʽ
Output a string with length $n_1$ on the first line. The $i$-th ($1\le i\le n_1$) character should be $1$ if the $i$-th rook placed by Prof. Pang is attacked and $0$ otherwise.

Output a string with length $n_2$ on the second line. The $i$-th ($1\le i\le n_2$) character should be $1$ if the $i$-th rook placed by Prof. Shou is attacked and $0$ otherwise.


```input1
3 2
0 0
0 1
1 0
0 -1
-1 0
```

```output1
100
11
```

