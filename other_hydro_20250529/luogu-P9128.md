## 题目描述
There are $N$ pastures $(2 \le N \le 2 \cdot 10^5)$, connected by $N−1$ roads, such that they form a tree. Every road takes $1$ second to cross. Each pasture starts out with $0$ grass, and the ith pasture's grass grows at a rate of $a_i (1 \le a_i \le 10^8)$ units per second. Farmer John is in pasture $1$ at the start, and needs to drive around and fertilize the grass in every pasture. If he visits a pasture with $x$ units of grass, it will need $x$ amount of fertilizer. A pasture only needs to be fertilized the first time it is visited, and fertilizing a pasture takes $0$ time.

The input contains an additional parameter $T \in \{0,1\}$.

 - If $T=0$, Farmer John must end at pasture $1$.
 - If $T=1$, Farmer John may end at any pasture.

Compute the minimum amount of time it will take to fertilize every pasture and the minimum amount of fertilizer needed to finish in that amount of time. 

## 输入格式
The first line contains $N$ and $T$.

Then for each $i$ from $2$ to $N$, there is a line containing $p_i$ and $a_i$, meaning that there is a road connecting pastures $p_i$ and $i$. It is guaranteed that $1 \le p_i<i$. 

## 输出格式
 The minimum amount of time and the minimum amount of fertilizer, separated by spaces. 

## 题目大意
### 题目描述

有 $N$ 个顶点的树，经过节点之间的每一条边都需要 $1s$。每个顶点一开始的权值均为 $0$，第 $i$ 个点的权值的增长速率为 $a_i/s$。FJ 从 $1$ 号顶点出发遍历整棵树。当 FJ 走到某个节点时，若该节点的权值为 $x$，则需要支出大小为 $x$ 的费用。（当然，只需在第一次经过该节点时需要支出。）

给出一个参数 $T$:

+ **若 $T=0$，FJ 必须回到 $1$ 号节点**。

+ **若 $T=1$，FJ 可以在任意节点结束他的遍历**。

求遍历所有节点的最小时间和此时需要付出的最小的费用。

### 输入格式

第一行包括 $N$ 和 $T$。

第 $2$ 行到第 $N$ 行，包含两个整数 $p_i$ 和 $a_i$,$a_i$ 的含义见上文。$p_i$ 则表示节点 $i$ 和 $p_i$ 之间有一条边相连。

### 输出格式
两个整数：遍历所有节点的最小时间和此时需要付出的最小的费用。

$2 \le N \le 2 \times 10^5,T \in \{0,1\},1 \le a_i \le 10^8, 1 \le p_i < i$。

```input1
5 0
1 1
1 2
3 1
3 4
```

```output1
8 21
```

```input2
5 1
1 1
1 2
3 1
3 4
```

```output2
6 29
```

## 提示
### Explanation for Sample 1

The optimal route for Farmer John is as follows: 

 - At time $1$, move to node $3$, which now has $1 \cdot 2=2$ grass and so needs $2$ fertilizer.
 - At time $2$, move to node $5$, which now has $2 \cdot 4=8$ grass and so needs $8$ fertilizer.
 - At time $3$, move back to node $3$, which we already fertilized and so don't need to fertilize again.
 - At time $4$, move to node $4$, which now has $4 \cdot 1=4$ grass and so needs $4$ fertilizer.
 - At time $5$, move back to node $3$, which we already fertilized.
 - At time $6$, move back to node $1$.
 - At time $7$, move to node $2$, which now has $7 \cdot 1=7$ grass and so needs $7$ fertilizer.
 - At time $8$, return to node $1$. 

This route takes $8$ time and uses $2+8+4+7=21$ fertilizer. It can be shown that $8$ is the least possible amount of time for any route that returns to node $1$ at the end and $21$ is the least possible fertilizer used for any route that returns to node $1$ and takes $8$ time.

### Explanation for Sample 2

The optimal route for Farmer John is as follows:

 - At time $1$, move to node $2$, which now has $1 \cdot 1=1$ grass and so needs $1$ fertilizer.
 - At time $2$, move back to node $1$.
 - At time $3$, move to node $3$, which now has $3 \cdot 2=6$ grass and so needs $6$ fertilizer.
 - At time $4$, move to node $5$, which now has $4 \cdot 4=16$ grass and so needs $16$ fertilizer.
 - At time $5$, move back to node $3$, which we already fertilized and so don't need to fertilize again.
 - At time $6$, move to node $4$, which now has $6 \cdot 1=6$ grass and so needs $6$ fertilizer.

This route takes $6$ time and uses $1+6+16+6=29$ fertilizer. It can be shown that $6$ is the least possible amount of time for any route and $29$ is the least possible fertilizer used for any route that takes $6$ time.

### SCORING

 - Inputs $3-10$: $T=0$
 - Inputs $11-22$: $T=1$
 - Inputs $3-6$ and $11-14$: No pasture is adjacent to more than three roads.

