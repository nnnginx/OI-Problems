## 题目描述
Prof. Pang is getting addicted to the game called Elden Ring, in which the world is a connected graph including $n$ vertices indexed from $1$ to $n$ and $m$ undirected edges. Players start at vertex $1$ and travel across the world to slay the god on vertex $n$.

However, it's not that easy. For any vertex $i$ except vertex $1$, there is exactly one boss whose level is $l_i$, and the player starts the game with level $l_1$. For each day, the player can travel to any vertex $i$ from vertex $1$ and challenge the boss there. If the current level of the player is greater than the boss, the boss will be eliminated from the world (inactivated) and the level of the player will be increased by $A$. Notice that traveling through a vertex that has an active boss is forbidden. (In other words, Prof. Pang can travel from vertex $1$ to vertex $i$ if there is a path in the graph from vertex $1$ to vertex $i$ such that each vertex on this path, except for vertex $i$, has no active boss.) Meanwhile, at the beginning of each day, all the remaining bosses in the world will also be promoted by $B$ levels.

To finish a playthrough of the game, you need to slay the boss on vertex $n$ (Elden Beast). Given the information of the world, Prof. Pang is wondering how many days he needs at least to do so. 

The Player can only challenge one boss each day.

## 输入格式
The first line contains a single integer $T~(1 \le T \le 10^5)$ denoting the number of test cases. 

For each test case, the first line includes four integers $n, m, A, B~(2\leq n\leq 2\times 10^5, 1 \le m, A, B\le 2\times 10^5)$. In next $m$ lines, each line contains two integers $a_i, b_i~(1 \le a_i, b_i \le n)$, denoting the endpoints of the $i$-th undirected edge. The last line contains $n$ integers $l_i~(1 \le l_i \le 2 \times 10^5)$, representing the initial levels of the player and bosses mentioned above.

It is guaranteed that the sum of $n$ over all test cases will not exceed $10^6$ and the sum of $m$ over all test cases will not exceed $10^6$.

## 输出格式
For each test case, output a single line containing an integer, indicating the minimum number of days Prof. Pang needs to finish the game. If it is impossible to do so, please output $-1$.

## 题目大意
有一个 $n$ 个节点 $m$ 条边的无向图，每个节点 $i$ 上有一个初始等级为 $l_i$ 的 boss。玩家开始时位于 1 号节点，初始等级为 $l_1$。（保证 1 号节点没有 boss）

每天开始后，玩家从 1 号节点开始，经过**没有 boss** 的节点到达一个有 boss 的节点 $i$，并击杀节点 $i$ 的 boss。玩家等级必须大于 boss 的等级才能将 boss 击杀，且每天只能击杀一个 boss。

每击杀一个 boss，玩家的等级会增加 $A$。每天开始时，所有**仍存在**的 boss 等级增加 $B$。输出至少需要多少天才能击杀节点 $n$ 的 boss 并通关，如果不能通关输出  -1 。

```input1
2
5 4 5 8
1 2
1 3
1 4
4 5
15 1 1 1 1
5 4 10 5
1 2
1 3
1 4
4 5
10 4 4 4 19

```

```output1
2
4

```

