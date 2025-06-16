## 题目描述
**Note: The time limit for this problem is 4s, 2x the default.**

To celebrate the start of spring, Farmer John's $N$ cows have invented an intriguing new dance, where they stand in a circle and re-order themselves in a predictable way.

Specifically, there are $N$ positions around the circle, numbered sequentially from $0$ to $N-1$, with position $0$ following position $N-1$.  A cow resides at each position.  The cows are also numbered sequentially from $0$ to $N-1$.  Initially, cow $i$ starts in position $i$.  You are told a set of $K$ positions $0=A_1<A_2<\dots<A_K<N$ that are "active", meaning the cows in these positions are the next to move.

In each minute of the dance, two things happen.  First, the cows in the active positions rotate: the cow at position $A_1$ moves to position $A_2$, the cow at position $A_2$ moves to position $A_3$, and so on, with the cow at position $A_K$ moving to position $A_1$.  All of these $K$ moves happen simultaneously, so the after the rotation is complete, all of the active positions still contain exactly one cow.  Next, the active positions themselves shift:
$A_1$ becomes $A_1+1$, $A_2$ becomes $A_2+1$, and so on (if $A_i = N-1$ for some active position, then $A_i$ circles back around to $0$).

Please calculate the order of the cows after $T$ minutes of the dance.

## 输入格式
The first line contains three integers $N, K$ and $T$.

The second line contains $K$ integers representing the initial set of active positions
$A_1,A_2, \dots, A_K$.  Recall that $A_1 = 0$ and that these are given in increasing order.

## 输出格式
Output the order of the cows after $T$ minutes, starting with the cow in position $0$, separated by
spaces.

## 题目大意
### 题目描述

**注意：本题的时间限制为 4 秒，是默认时间限制的 2 倍。**

为了庆祝春天的到来，Farmer John 的 $N$ 头奶牛发明了一种有趣的舞蹈，她们围成一个圆圈，并以一种可预测的方式重新排列自己。

具体来说，圆圈上有 $N$ 个位置，编号从 $0$ 到 $N-1$，其中位置 $0$ 紧接着位置 $N-1$。每个位置上有一头奶牛。奶牛的编号也从 $0$ 到 $N-1$。初始时，奶牛 $i$ 位于位置 $i$。你会被告知一组 $K$ 个“活跃”位置 $0 = A_1 < A_2 < \dots < A_K < N$，这意味着这些位置上的奶牛是下一批要移动的。

在舞蹈的每一分钟，会发生两件事。首先，活跃位置上的奶牛会旋转：位置 $A_1$ 的奶牛移动到位置 $A_2$，位置 $A_2$ 的奶牛移动到位置 $A_3$，依此类推，位置 $A_K$ 的奶牛移动到位置 $A_1$。所有这些 $K$ 次移动同时发生，因此在旋转完成后，所有活跃位置仍然恰好有一头奶牛。接下来，活跃位置本身会移动：$A_1$ 变为 $A_1 + 1$，$A_2$ 变为 $A_2 + 1$，依此类推（如果某个活跃位置 $A_i = N-1$，则 $A_i$ 会循环回到 $0$）。

请计算舞蹈进行 $T$ 分钟后奶牛的顺序。

### 输入格式

第一行包含三个整数 $N$、$K$ 和 $T$。

第二行包含 $K$ 个整数，表示初始的活跃位置 $A_1, A_2, \dots, A_K$。注意 $A_1 = 0$，并且这些位置是按递增顺序给出的。

### 输出格式

输出 $T$ 分钟后奶牛的顺序，从位置 $0$ 的奶牛开始，用空格分隔。

### 提示

对于上述样例，以下是前四个时间步的奶牛顺序和活跃位置 $A$：
```
初始，T = 0：顺序 = [0 1 2 3 4]，A = [0 2 3]
T = 1：顺序 = [3 1 0 2 4]
T = 1：A = [1 3 4]
T = 2：顺序 = [3 4 0 1 2]
T = 2：A = [2 4 0]
T = 3：顺序 = [2 4 3 1 0]
T = 3：A = [3 0 1]
T = 4：顺序 = [1 2 3 4 0]
```

$1 \leq K \leq N \leq 2 \cdot 10^5$，$1 \leq T \leq 10^9$。

- 输入 2-7：$N \leq 1000$，$T \leq 10000$。
- 输入 8-13：没有额外限制。

```input1
5 3 4
0 2 3

```

```output1
1 2 3 4 0

```

## 提示
For the example above, here are the cow orders and $A$ for the first four timesteps:
```
Initial, T = 0: order = [0 1 2 3 4], A = [0 2 3]
T = 1: order = [3 1 0 2 4]
T = 1: A = [1 3 4]
T = 2: order = [3 4 0 1 2]
T = 2: A = [2 4 0]
T = 3: order = [2 4 3 1 0]
T = 3: A = [3 0 1]
T = 4: order = [1 2 3 4 0]
```

$1 \leq K \leq N \leq 2 \cdot 10^5$, $1\le T\le 10^9$.

- Inputs 2-7: $N \leq 1000, T \leq 10000$.
- Inputs 8-13: No additional constraints.

