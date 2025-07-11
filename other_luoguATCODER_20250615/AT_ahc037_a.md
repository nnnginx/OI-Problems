# AT_ahc037_a [AHC037A] Soda

## 题目描述

碳酸饮料的**甜度**和**碳酸强度**分别表示为非负整数。饮料的甜度为 $x$、碳酸强度为 $y$ 时，记为 $(x, y)$。

刚开始，你仅有一种饮料 $(0, 0)$。记已经制作出的饮料集合为 $S$，起初 $S = \{(0, 0)\}$。

你可以重复以下操作来制作更多种类的饮料：

1. 从集合 $S$ 中选择一瓶饮料 $(x, y)$；
2. 选择满足 $x' \ge x$ 和 $y' \ge y$ 的整数 $x', y'$；
3. 将 $(x, y)$ 分成两部分，一部分保持不变，另一部分通过添加糖浆和碳酸制作成新的饮料 $(x', y')$，然后将 $(x', y')$ 添加到 $S$ 中。
   - 注意，$(x, y)$ 并不会从集合 $S$ 中移除。
4. 该操作的代价为 $(x' - x) + (y' - y)$。

输入包含 $N$ 种指定的饮料 $(A_1, B_1), \dots, (A_N, B_N)$。你需要在最多 $5N$ 次操作内，找到一种制作出所有指定饮料的操作序列，同时使总代价尽可能小。操作过程中，有权制作一些未在输入中给出的饮料。

## 输入格式

输入按照如下格式给出：

> $N$ $A_1$ $B_1$ $\vdots$ $A_N$ $B_N$

所有输入均为整数，满足以下约束条件：

- $N = 1000$
- $0 \le A_i < 10^9$
- $0 \le B_i < 10^9$
- $A_1, A_2, \dots, A_N$ 两两不同
- $B_1, B_2, \dots, B_N$ 两两不同
- 存在某个 $i$ 使得 $A_i = 0$
- 存在某个 $i$ 使得 $B_i = 0$

## 输出格式

若执行的操作次数为 $M$，并在第 $m$ 次操作中从 $(x_m, y_m)$ 制作出 $(x'_m, y'_m)$，则输出应为：

> $M$ $x_1$ $y_1$ $x'_1$ $y'_1$ $\vdots$ $x_M$ $y_M$ $x'_M$ $y'_M$

所有输出均为整数，并需满足以下条件：

- $0 \le M \le 5N$
- $0 \le x_m \le x'_m < 10^9$ 且 $0 \le y_m \le y'_m < 10^9$
- 对于任意 $(x_m, y_m) \ne (0, 0)$，存在 $k < m$ 使得 $(x_m, y_m) = (x'_k, y'_k)$
- 对于任意 $(A_i, B_i) \ne (0, 0)$，存在某个操作 $m$ 使得 $(A_i, B_i) = (x'_m, y'_m)$

此外，如果存在代价为 $C$ 的操作序列不满足 $M \le 5N$ 的条件，则一定存在代价不大于 $C$ 的操作序列满足所有条件。

## 得分说明

总代价记为 $C$，$L = \max\{A_1, B_1, A_2, B_2, \dots, A_N, B_N\}$。得分按以下公式计算：$\mathrm{round}\left(10^6 \times \frac{NL}{1 + C}\right)$。

共有 150 个测试用例，总得分为各测试用例得分之和。若某测试用例输出不合法或超时，则整体提交结果为错误 (WA) 或超时 (TLE)。比赛结束后不进行系统测试。得分相同者排名一致，与提交时间无关。

 **本翻译由 AI 自动生成**

## 输入输出样例 #1

### 输入 #1

```
4
0 6
2 5
3 2
4 0
```

### 输出 #1

```
6
0 0 2 0
0 0 0 6
2 0 4 0
2 0 2 2
2 2 3 2
2 2 2 5
```