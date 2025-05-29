## 题目描述
It's winter on the farm, and that means snow! There are $N$ tiles on the path from the farmhouse to the barn, conveniently numbered $1 \dots N$, and tile $i$ is covered in $f_i$ feet of snow.
Farmer John starts off on tile $1$ and must reach tile $N$ to wake up the cows. Tile $1$ is sheltered by the farmhouse roof, and tile $N$ is sheltered by the barn roof, so neither of these tiles has any snow. But to step on the other tiles, Farmer John needs to wear boots!

In his foul-weather backpack, Farmer John has $B$ pairs of boots, numbered $1 \dots B$. Some pairs are more heavy-duty than others, and some pairs are more agile than others. In particular, pair $i$ lets FJ step in snow at most $s_i$ feet deep, and lets FJ move at most $d_i$ forward in each step.

Unfortunately, the boots are packed in such a way that Farmer John can only access the topmost pair at any given time. So at any time, Farmer John can either put on the topmost pair of boots (discarding his old pair) or discard the topmost pair of boots (making a new pair of boots accessible).

Farmer John can only change boots while standing on a tile. If that tile has $f$ feet of snow, both the boots he takes off AND the boots he puts on must be able to withstand at least $f$ feet of snow. Intermediate pairs of boots which he discards without wearing do not need to satisfy this restriction.

Help Farmer John minimize waste, by determining the minimum number of pairs of boots he needs to discard in order to reach the barn. You may assume that Farmer John is initially not wearing any boots.

## 输入格式
The first line contains two space-separated integers $N$ and $B$ ($2 \leq N,B \leq 250$).
The second line contains $N$ space-separated integers. The $i$th integer is $f_i$, giving the depth of snow on tile $i$ ($0 \leq f_i \leq 10^9$). It's guaranteed that $f_1 = f_N = 0$.

The next $B$ lines contain two space-separated integers each. The first integer on line $i+2$ is $s_i$, the maximum depth of snow in which pair $i$ can step. The second integer on line $i+2$ is $d_i$, the maximum step size for pair $i$. It's guaranteed that $0 \leq s_i \leq 10^9$ and $1 \leq d_i \leq N-1$.

The boots are described in top-to-bottom order, so pair $1$ is the topmost pair in FJ's backpack, and so forth.

## 输出格式
The output should consist of a single integer, giving the minimum number of boots Farmer John needs to discard. It's guaranteed that it will be possible for FJ to make it to the barn.

## 题目大意
### 题目描述

农场的冬天到了，这意味着下雪了！从农舍到谷仓的路上有 $N$ 块地砖，方便地编号为 $1 \dots N$，第 $i$ 块地砖上覆盖了 $f_i$ 英尺的雪。

Farmer John 从第 $1$ 块地砖出发，必须到达第 $N$ 块地砖去叫醒奶牛。第 $1$ 块地砖被农舍的屋顶遮蔽，第 $N$ 块地砖被谷仓的屋顶遮蔽，因此这两块地砖上没有雪。但要踩在其他地砖上，Farmer John 需要穿靴子！

在他的恶劣天气背包中，Farmer John 有 $B$ 双靴子，编号为 $1 \dots B$。有些靴子比其他靴子更耐用，有些靴子比其他靴子更灵活。具体来说，第 $i$ 双靴子允许 Farmer John 在最多 $s_i$ 英尺深的雪中行走，并且每步最多可以移动 $d_i$ 块地砖。

不幸的是，靴子的打包方式使得 Farmer John 在任何时候只能访问最上面的一双靴子。因此，Farmer John 可以随时穿上最上面的一双靴子（丢弃旧靴子）或丢弃最上面的一双靴子（使下一双靴子可访问）。

Farmer John 只能在地砖上更换靴子。如果该地砖上有 $f$ 英尺的雪，那么他脱下的靴子和穿上的靴子都必须能够承受至少 $f$ 英尺的雪。他丢弃但未穿过的中间靴子不需要满足此限制。

请帮助 Farmer John 最小化浪费，确定他到达谷仓需要丢弃的最少靴子对数。假设 Farmer John 最初没有穿任何靴子。

### 输入格式

第一行包含两个以空格分隔的整数 $N$ 和 $B$（$2 \leq N, B \leq 250$）。

第二行包含 $N$ 个以空格分隔的整数。第 $i$ 个整数是 $f_i$，表示第 $i$ 块地砖上的雪的深度（$0 \leq f_i \leq 10^9$）。保证 $f_1 = f_N = 0$。

接下来的 $B$ 行每行包含两个以空格分隔的整数。第 $i+2$ 行的第一个整数是 $s_i$，表示第 $i$ 双靴子可以承受的最大雪深。第二个整数是 $d_i$，表示第 $i$ 双靴子的最大步长。保证 $0 \leq s_i \leq 10^9$ 且 $1 \leq d_i \leq N-1$。

靴子按从上到下的顺序描述，因此第 $1$ 双靴子是背包中最上面的一双，依此类推。

### 输出格式

输出应包含一个整数，表示 Farmer John 需要丢弃的最少靴子对数。保证 Farmer John 能够到达谷仓。

### 提示

题目来源：Brian Dean 和 Dhruv Rohatgi

```input1
10 4
0 2 8 3 6 7 5 1 4 0
2 3
4 2
3 4
7 1
```

```output1
2

```

## 提示
Problem credits: Brian Dean and Dhruv Rohatgi

