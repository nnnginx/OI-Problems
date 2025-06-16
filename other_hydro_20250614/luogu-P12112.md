## 题目描述
The $\textit{Towers of Hanoi}$ is a famous mathematical puzzle consisting of three rods and $n$ disks with diameters $1, 2, \ldots, n$. Each of the three rods contains some disks, stacked in order of decreasing diameter from bottom to top, so that the smallest disk is always at the top. A valid move consists of taking the smallest disk from a rod and putting it on top of another rod. This move must preserve the sorted order: you can't put a larger disk onto a smaller one. The original puzzle's goal is to transfer all disks from one rod to another.

In this variation of the puzzle, you can only move the disks $\textbf{between adjacent rods}$: you can move a disk between rods $1$ and $2$, and between rods $2$ and $3$, but not between rods $1$ and $3$.

![](https://cdn.luogu.com.cn/upload/image_hosting/8p2sy9bm.png)

Given two configurations of this puzzle, find the minimum number of moves required to reach the second configuration starting from the first one. As this number might be large, print it modulo $998\,244\,353$.

## 输入格式
Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^3$). Descriptions of the test cases follow.

The first line of each test case contains an integer $n$, denoting the number of disks involved ($1 \le n \le 10^5$).

The second line contains $n$ integers $x_1, x_2, \ldots, x_n$, describing the initial configuration of the puzzle, where $x_i$ is the rod that contains the $i$-th disk ($x_i \in \{ 1, 2, 3 \}$).

The third line describes the final configuration of the puzzle in the same format.

It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.

## 输出格式
For each test case, print the minimum number of moves required to reach the second configuration from the first one, modulo $998\,244\,353$.

It can be shown that any two configurations are reachable from each other in this variation of the puzzle.

```input1
4
1
1
3
2
3 3
2 1
3
3 2 1
1 2 3
4
2 1 3 2
2 1 3 2
```

```output1
2
7
20
0
```

