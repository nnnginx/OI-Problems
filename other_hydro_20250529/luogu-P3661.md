## 题目描述
Farmer John's cows are trying to learn to cross the road effectively. Remembering the old "why did the chicken cross the road?" joke, they figure the chickens must be experts on crossing the road, and go off in search of chickens to help them.

As it turns out, chickens are very busy creatures and have limited time to help the cows. There are $C$ chickens on the farm ($1 \leq C \leq 20,000$), conveniently numbered $1 \ldots C$, and each chicken $i$ is only willing to help a cow at precisely time $T_i$. The cows, never in a hurry, have more flexibility in their schedules. There are $N$ cows on the farm ($1 \leq N \leq 20,000$), conveniently numbered $1 \ldots N$, where cow $j$ is able to cross the road between time $A_j$ and time $B_j$. Figuring the "buddy system" is the best way to proceed, each cow $j$ would ideally like to find a chicken $i$ to help her cross the road; in order for their schedules to be compatible, $i$ and $j$ must satisfy $A_j \leq T_i \leq B_j$.

If each cow can be paired with at most one chicken and each chicken with at most one cow, please help compute the maximum number of cow-chicken pairs that can be constructed.

## 输入格式
The first line of input contains $C$ and $N$. The next $C$ lines contain $T_1 \ldots T_C$, and the next $N$ lines contain $A_j$ and $B_j$ ($A_j \leq B_j$) for $j = 1 \ldots N$. The $A$'s, $B$'s, and $T$'s are all non-negative integers (not necessarily distinct) of size at most 1,000,000,000

## 输出格式
Please compute the maximum possible number of cow-chicken pairs.


## 题目大意
### 题目描述

Farmer John 的奶牛们正在学习如何有效地过马路。回想起古老的“鸡为什么要过马路？”笑话，他们认为鸡一定是过马路的专家，于是去寻找鸡来帮助它们。

事实上，鸡是非常忙碌的生物，它们只有有限的时间来帮助奶牛。农场上有 $C$ 只鸡（$1 \leq C \leq 20,000$），方便地用编号 $1 \ldots C$ 标识，每只鸡 $i$ 只愿意在确切的时间 $T_i$ 帮助一头奶牛。奶牛们从不着急，它们的日程安排更加灵活。农场上有 $N$ 头奶牛（$1 \leq N \leq 20,000$），方便地用编号 $1 \ldots N$ 标识，其中奶牛 $j$ 能够在时间 $A_j$ 到时间 $B_j$ 之间过马路。考虑到“伙伴系统”是最好的方式，每头奶牛 $j$ 理想情况下希望找到一只鸡 $i$ 来帮助她过马路；为了使它们的日程安排兼容，$i$ 和 $j$ 必须满足 $A_j \leq T_i \leq B_j$。

如果每头奶牛最多只能与一只鸡配对，每只鸡也最多只能与一头奶牛配对，请计算可以构建的最大奶牛-鸡配对数。

### 输入格式

输入的第一行包含 $C$ 和 $N$。接下来的 $C$ 行包含 $T_1 \ldots T_C$，接下来的 $N$ 行包含 $A_j$ 和 $B_j$（$A_j \leq B_j$），其中 $j = 1 \ldots N$。$A$、$B$ 和 $T$ 都是不超过 1,000,000,000 的非负整数（不一定互不相同）。

### 输出格式

请计算可能的奶牛-鸡配对的最大数量。

```input1
5 4
7
8
6
2
9
2 5
4 9
0 3
8 13
```

```output1
3
```

