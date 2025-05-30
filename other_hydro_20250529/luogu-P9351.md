## 题目描述
President K loves solving mazes. He found cells from which he may create a maze. The cells are rectangular grid with $R$ horizontal rows and $C$ vertical columns. Each cell is colored either white or black. The cell in the $i$-th row ($1 \leqslant i \leqslant R$) from the top and the $j$-th column ($1 \leqslant j \leqslant C$) from the left is called Cell $(i, j)$.

President K will solve the maze under the condition that he can pass the white cells, but he cannot pass the black cells. More precisely, he will solve the maze in the following way.

1. Among the white cells, he will choose Cell $(S_r, S_c)$, which is the starting cell of the maze, and Cell $(G_r, G_c)$, which is the goal cell of the maze.
2. It is possible to move from one cell to another white cell which is adjacent to the current cell in one of the four directions (top, bottom, left, or right). By repeating this, he will find a path from the starting cell to the goal cell.

President K already fixed the starting cell and the goal cell. However, he noticed that in some situations of the colors of the cells, there might not be a path from the starting cell to the goal cell consisting of white cells only. He has a stamp of size $N \times N$. He will perform the following **Operations** several times so that there will be a path from the starting cell to the goal cell consisting of white cells only.

**Operation.** He chooses a square region of $N \times N$ cells, and paint the cells in the region white. More precisely, he chooses integers $a, b$ satisfying $1 \leqslant a \leqslant R - N + 1$ and $1 \leqslant b \leqslant C − N + 1$, and for every pair $(i, j)$ of integers satisfying $a \leqslant i \leqslant a + N − 1$ and $b \leqslant j \leqslant b + N − 1$, he paints Cell $(i, j)$ white.

Since his hands becomes dirty if he uses the stamp, he wants to minimize the number of operations. Given
information of the colors of the cells, the size of the stamp, and the locations of the starting cell and the goal cell, write a program which calculates the minimum number of operations he has to perform so that there will be a path from the starting cell to the goal cell consisting of white cells only.

## 输入格式
Read the following data from the standard input.

> $R$ $C$ $N$  
$S_r$ $S_c$  
$G_r$ $G_c$  
$A_1$  
$A_2$  
$.$  
$.$  
$.$  
$A_R$

$A_i (1 \leqslant i \leqslant R)$ is a string of length $C$ consisting of `.` or `#`. The $j$-th character ($1 \leqslant j \leqslant C$) of $A_i$ represents the color of Cell $(i, j)$. Its color is white if the character is `.`, and its color is black if the character is `#`.

## 输出格式
Write one line to the standard output. The output should contain the minimum number of operations President
K has to perform so that there will be a path from the starting cell to the goal cell consisting of white cells only.

## 题目大意
给定一张 $R\times C$ 的地图，其中 ```.``` 可以走，而 ```#``` 不能走。一次操作可以将 $N \times N$ 的正方形范围内所有点变成 ```.```，给定起点和终点，求最少需要几次操作使得起点和终点连通（只能上下左右移动）。

$R\times C\le 6\times 10^6$，$N\le R\le C$。

```input1
2 4 2
1 1
2 4
.###
###.

```

```output1
1

```

```input2
6 6 1
1 6
6 1
..#.#.
##.###
####.#
...###
##.##.
.#.###

```

```output2
4

```

```input3
6 7 6
6 4
3 1
..#.#.#
##.##..
.######
#..#.#.
.######
..#.##.

```

```output3
1

```

```input4
1 15 1
1 15
1 1
...............

```

```output4
0

```

## 提示
#### 【样例解释 #1】

If he chooses $(a, b) = (1, 2)$ and perform an operation, Cells $(1, 2), (1, 3), (2, 2), (2, 3)$ become white. Then there will be a path from the starting cell to the goal cell consisting of white cells only. For example, the path $(1, 1) → (1, 2) → (1, 3) → (2, 3) → (2, 4)$ satisfies the condition.

If he does not perform an operation, there is no path from the starting cell to the goal cell consisting of white cells only. Therefore, output $1$.

该样例满足子任务 $2, 3, 4, 5, 6, 7, 8$ 的限制。

#### 【样例解释 #2】

该样例满足所有子任务的限制。

#### 【样例解释 #3】

该样例满足子任务 $2, 3, 4, 5, 6, 7, 8$ 的限制。

#### 【样例解释 #4】

Even if he does not perform an operation, there might be a path from the starting cell to the goal cell consisting of white cells only.

该样例满足所有子任务的限制。

#### 【数据范围】

对于所有测试数据，满足 $1 ≤ N ≤ R ≤ C$, $R × C ≤ 6 \times 10^6$, $1 ≤ S_r ≤ R$, $1 ≤ S_c ≤ C$, $1 ≤ G_r ≤ R$, $1 ≤ G_c ≤ C$, $(S_r, S_c) \neq (G_r, G_c)$.

保证 $A_i (1 ≤ i ≤ R)$ 是一个长为 $C$ 且只由 `.` 或 `#` 构成的字符串。保证格子 $(S_r, S_c)$ 与格子 $(G_r, G_c)$ 均为白色。

保证 $R, C, N, S_r, S_c, G_r, G_c$ 均为整数。

| 子任务编号 | 分值 | 限制 |
| :-: | :-: | :-: |
| $1$ | $8$ | $N = 1, R × C ≤ 1.5 \times 10^6$ |
| $2$ | $19$ | $R × C ≤ 10^3$ |
| $3$ | $16$ | 答案不超过 $10$, $R × C ≤ 1.5 \times 10^6$ |
| $4$ | $19$ | $R × C ≤ 6 \times 10^4$ |
| $5$ | $5$ | $R × C ≤ 1.5 \times 10^5$ |
| $6$ | $19$ | $R × C ≤ 1.5 \times 10^6$ |
| $7$ | $8$ | $R × C ≤ 3 \times 10^6$ |
| $8$ | $6$ | 无 |

