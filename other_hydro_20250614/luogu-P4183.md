## 题目描述
Cornered at last, Bessie has gone to ground in a remote farm. The farm consists of $N$ barns ($2 \leq N \leq 7 \cdot 10^4$) and $N-1$ bidirectional tunnels between barns, so that there is a unique path between every pair of barns. Every barn which has only one tunnel is an exit. When morning comes, Bessie will surface at some barn and attempt to reach an exit.

But the moment Bessie surfaces at some barn, the law will be able to pinpoint her location. Some farmers will then start at various exit barns, and attempt to catch Bessie. The farmers move at the same speed as Bessie (so in each time step, each farmer can move from one barn to an adjacent barn). The farmers know where Bessie is at all times, and Bessie knows where the farmers are at all times. The farmers catch Bessie if at any instant a farmer is in the same barn as Bessie, or crossing the same tunnel as Bessie. Conversely, Bessie escapes if she reaches an exit barn strictly before any farmers catch her.


Bessie is unsure at which barn she should surface. For each of the $N$ barns, help Bessie determine the minimum number of farmers who would be needed to catch Bessie if she surfaced there, assuming that the farmers distribute themselves optimally among the exit barns.


Note that the time limit for this problem is slightly larger than the default: 4 seconds for C/C++/Pascal, and 8 seconds for Java/Python.


## 输入格式
The first line of the input contains $N$. Each of the following $N-1$ lines specify two integers, each in the range $1 \ldots N$, describing a tunnel between two barns.


## 输出格式
Please output $N$ lines, where the $i$th line of output tells the minimum number of farmers necessary to catch Bessie if she surfaced at the $i$th barn.


## 题目大意
### 题目描述

Bessie 被逼到了绝境，躲进了一个偏远的农场。这个农场由 $N$ 个谷仓（$2 \leq N \leq 7 \cdot 10^4$）和 $N-1$ 条双向隧道组成，因此每对谷仓之间都有一条唯一的路径。每个只有一个隧道的谷仓都是一个出口。当早晨来临时，Bessie 会从某个谷仓出现，并试图到达一个出口。

但是，当 Bessie 从某个谷仓出现时，执法人员会立即定位到她的位置。一些农民会从各个出口谷仓出发，试图抓住 Bessie。农民和 Bessie 的移动速度相同（因此在每个时间步中，每个农民可以从一个谷仓移动到相邻的谷仓）。农民们始终知道 Bessie 的位置，而 Bessie 也始终知道农民们的位置。如果农民和 Bessie 在同一谷仓或同时穿过同一条隧道，农民就会抓住 Bessie。相反，如果 Bessie 在农民抓住她之前严格地到达一个出口谷仓，她就能逃脱。

Bessie 不确定她应该从哪个谷仓出现。对于每个谷仓，请帮助 Bessie 确定如果她从该谷仓出现，假设农民们最优地分布在出口谷仓中，抓住她所需的最少农民数量。

请注意，本题的时间限制略高于默认值：C/C++/Pascal 为 4 秒，Java/Python 为 8 秒。

### 输入格式

输入的第一行包含 $N$。接下来的 $N-1$ 行每行包含两个整数，范围在 $1 \ldots N$ 之间，描述一条连接两个谷仓的隧道。

### 输出格式

请输出 $N$ 行，其中第 $i$ 行表示如果 Bessie 从第 $i$ 个谷仓出现，抓住她所需的最少农民数量。

```input1
7
1 2
1 3
3 4
3 5
4 6
5 7
```

```output1
3
1
3
3
3
1
1
```

