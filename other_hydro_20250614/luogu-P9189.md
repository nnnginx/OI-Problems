## 题目描述
Due to the disorganized structure of his mootels (much like motels but with
bovine rather than human guests), Farmer John has decided to take up the role of
the mootel custodian to restore order to the stalls.

Each mootel has $N$ stalls labeled $1$ through $N$ and $M$ corridors that connect pairs of stalls to each other
bidirectionally. The $i$ th stall is painted with color $C_i$ and initially has a
single key of color $S_i$ in it. FJ will have to rearrange the keys to appease
the cows and restore order to the stalls.

FJ starts out in stall $1$ without holding any keys and is allowed to repeatedly
do one of the following moves:
- Pick up a key in the stall he is currently in. FJ can hold multiple keys at
a time.
- Place down a key he is holding into the stall he is currently
in. A stall may hold multiple keys at a time.
- Enter stall $1$ by
moving through a corridor.
- Enter a stall other than stall $1$ by
moving through a corridor. He can only do this if he currently holds a key that
is the same color as the stall he is entering.

Unfortunately, it seems that the keys are not in their intended locations. To
restore order to FJ's mootel, the $i$th stall requires that a single key of
color $F_i$ is in it. It is guaranteed that $S$ is a permutation of $F$.

For $T$ different mootels, FJ starts in stall $1$ and needs
to place every key in its appropriate location, ending back in stall $1$. For
each of the $T$ mootels, please answer if it is possible to do this.

## 输入格式
The first line contains $T$, the number of mootels (test cases).

Each test case will be preceded by a blank line. Then, the first line 
of each test case contains two integers $N$ and $M$.

The second line of each test case contains $N$ integers. The $i$-th integer on
this line $C_i$ means that stall $i$ has color $C_i$.

The third line of each test case contains $N$ integers. The $i$-th integer on
this line $S_i$ means that stall $i$ initially holds a key of color $S_i$.

The fourth line of each test case contains $N$ integers. The $i$-th integer on
this line $F_i$ means that stall $i$ needs to have a key of color $F_i$ in it.

The next $M$ lines of each test case follow. The $i$-th of these lines contains
two distinct integers $u_i$ and $v_i$. This represents
that a corridor exists between stalls $u_i$ and $v_i$. No corridors are
repeated.


## 输出格式
For each mootel, output `YES` on a new line if there exists a way for FJ to return
a key of color $F_i$ to each stall $i$ and end back in stall $1$. Otherwise,
output `NO` on a new line.

## 题目大意
### 题目描述

由于他的 mootels（类似于汽车旅馆，但住客是牛而不是人）结构混乱，农夫 John 决定担任 mootel 的管理员，以恢复牛栏的秩序。

每个 mootel 有 $N$ 个牛栏，编号为 $1$ 到 $N$，以及 $M$ 条双向连接的走廊。第 $i$ 个牛栏被涂成颜色 $C_i$，并且最初里面有一把颜色为 $S_i$ 的钥匙。FJ 需要重新安排钥匙的位置，以安抚奶牛并恢复牛栏的秩序。

FJ 从牛栏 $1$ 开始，手中没有任何钥匙，并且可以重复执行以下操作之一：
- 拾取当前所在牛栏中的一把钥匙。FJ 可以同时持有多个钥匙。
- 将手中持有的一把钥匙放入当前所在的牛栏。一个牛栏可以同时存放多把钥匙。
- 通过走廊进入牛栏 $1$。
- 通过走廊进入牛栏 $1$ 以外的其他牛栏。只有当 FJ 当前持有的钥匙颜色与目标牛栏的颜色相同时，才能执行此操作。

不幸的是，钥匙似乎并未放在它们应有的位置。为了恢复 FJ 的 mootel 的秩序，第 $i$ 个牛栏需要有一把颜色为 $F_i$ 的钥匙。保证 $S$ 是 $F$ 的一个排列。

对于 $T$ 个不同的 mootel，FJ 从牛栏 $1$ 开始，需要将每把钥匙放到其应有的位置，并最终回到牛栏 $1$。对于每个 mootel，请回答是否可能完成这一任务。

### 输入格式

第一行包含 $T$，表示 mootel 的数量（测试用例的数量）。

每个测试用例前有一个空行。然后，每个测试用例的第一行包含两个整数 $N$ 和 $M$。

每个测试用例的第二行包含 $N$ 个整数。第 $i$ 个整数 $C_i$ 表示牛栏 $i$ 的颜色为 $C_i$。

每个测试用例的第三行包含 $N$ 个整数。第 $i$ 个整数 $S_i$ 表示牛栏 $i$ 最初有一把颜色为 $S_i$ 的钥匙。

每个测试用例的第四行包含 $N$ 个整数。第 $i$ 个整数 $F_i$ 表示牛栏 $i$ 需要有一把颜色为 $F_i$ 的钥匙。

每个测试用例接下来的 $M$ 行，每行包含两个不同的整数 $u_i$ 和 $v_i$。这表示牛栏 $u_i$ 和 $v_i$ 之间有一条走廊。没有重复的走廊。

### 提示

对于第一个样例的第一个测试样例，以下是一种可能的操作序列。

```
当前牛栏：1。持有的钥匙：[]。牛栏中的钥匙：[3, 4, 3, 4, 2] （拾取颜色为 3 的钥匙）
当前牛栏：1。持有的钥匙：[3]。牛栏中的钥匙：[x, 4, 3, 4, 2] （从牛栏 1 移动到牛栏 2，允许，因为持有颜色为 C_2=3 的钥匙）
当前牛栏：2。持有的钥匙：[3]。牛栏中的钥匙：[x, 4, 3, 4, 2] （拾取颜色为 4 的钥匙）
当前牛栏：2。持有的钥匙：[3, 4]。牛栏中的钥匙：[x, x, 3, 4, 2] （从牛栏 2 移动到牛栏 1 到牛栏 4 到牛栏 5，允许，因为持有颜色为 C_4=4 和 C_5=3 的钥匙）
当前牛栏：5。持有的钥匙：[3, 4]。牛栏中的钥匙：[x, x, 3, 4, 2] （拾取颜色为 2 的钥匙并放下颜色为 3 的钥匙）
当前牛栏：5。持有的钥匙：[2, 4]。牛栏中的钥匙：[x, x, 3, 4, 3] （从牛栏 5 移动到牛栏 4 到牛栏 1 到牛栏 3，允许，因为持有颜色为 C_4=4 和 C_3=2 的钥匙）
当前牛栏：3。持有的钥匙：[2, 4]。牛栏中的钥匙：[x, x, 3, 4, 3] （拾取颜色为 3 的钥匙并放下颜色为 4 的钥匙）
当前牛栏：3。持有的钥匙：[2, 3]。牛栏中的钥匙：[x, x, 4, 4, 3] （从牛栏 3 移动到牛栏 2 并放下颜色为 3 的钥匙）
当前牛栏：2。持有的钥匙：[2]。牛栏中的钥匙：[x, 3, 4, 4, 3] （从牛栏 2 移动到牛栏 1 并放下颜色为 2 的钥匙）
当前牛栏：1。持有的钥匙：[]。牛栏中的钥匙：[2, 3, 4, 4, 3]
```

对于第一个样例的第二个测试用例，不存在一种方式让 FJ 将颜色为 $F_i$ 的钥匙放回每个牛栏 $i$ 并最终回到牛栏 $1$。

$0 \le M \le 10^5$，$1 \le C_i, S_i, F_i, u_i, v_i \le N \le 10^5$。  
$1 \le T \le 100$，$1 \le \sum N \le 10^5$，$1 \le \sum M \le 2 \cdot 10^5$。

- 测试用例 3-6 满足 $N, M \le 8$。
- 测试用例 7-10 满足 $C_i = F_i$。
- 测试用例 11-18 没有额外限制。

```input1
2

5 5
4 3 2 4 3
3 4 3 4 2
2 3 4 4 3
1 2
2 3
3 1
4 1
4 5

4 3
3 2 4 1
2 3 4 4
4 2 3 4
4 2
4 1
4 3

```

```output1
YES
NO

```

```input2
5

2 0
1 2
2 2
2 2

2 1
1 1
2 1
2 1
1 2

2 1
1 1
2 1
1 2
1 2

2 1
1 1
1 2
2 1
1 2

5 4
1 2 3 4 4
2 3 5 4 2
5 3 2 4 2
1 2
1 3
1 4
4 5

```

```output2
YES
YES
NO
YES
NO

```

## 提示
For the first test case of the first sample, here is a possible sequence of moves:

```
Current stall: 1. Keys held: []. Keys in stalls: [3, 4, 3, 4, 2]
(pick up key of color 3)
Current stall: 1. Keys held: [3]. Keys in stalls: [x, 4, 3, 4, 2]
(move from stall 1 to 2, allowed since we have a key of color C_2=3)
Current stall: 2. Keys held: [3]. Keys in stalls: [x, 4, 3, 4, 2]
(pick up key of color 4)
Current stall: 2. Keys held: [3, 4]. Keys in stalls: [x, x, 3, 4, 2]
(move from stall 2 to 1 to 4 to 5, allowed since we have keys of colors C_4=4 and C_5=3)
Current stall: 5. Keys held: [3, 4]. Keys in stalls: [x, x, 3, 4, 2]
(pick up key of color 2 and place key of color 3)
Current stall: 5. Keys held: [2, 4]. Keys in stalls: [x, x, 3, 4, 3]
(move from stall 5 to 4 to 1 to 3, allowed since we have keys of colors C_4=4 and C_3=2)
Current stall: 3. Keys held: [2, 4]. Keys in stalls: [x, x, 3, 4, 3]
(pick up key of color 3 and place key of color 4)
Current stall: 3. Keys held: [2, 3]. Keys in stalls: [x, x, 4, 4, 3]
(move from stall 3 to stall 2 and place key of color 3)
Current stall: 2. Keys held: [2]. Keys in stalls: [x, 3, 4, 4, 3]
(move from stall 2 to stall 1 and place key of color 2)
Current stall: 1. Keys held: []. Keys in stalls: [2, 3, 4, 4, 3]
```

For the second test case of the first sample, there exists no way for FJ to return a key of color
$F_i$ to each stall $i$ and end back at stall $1$.

$0 \le M \le 10^5$, $1 \le C_i, S_i, F_i, u_i, v_i \le N \le 10^5$.   
$1 \le T \le 100$, $1 \le \sum N \le 10^5$, $1 \le \sum M \le 2\cdot 10^5$.

- Test cases 3-6 satisfy $N,M\le 8$.
- Test cases 7-10 satisfy $C_i=F_i$.
- Test cases 11-18 satisfy no additional constraints.


