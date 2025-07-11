# AT_arc191_e [ARC191E] Unfair Game

## 题目描述

给定正整数 $N, X, Y$ 以及长度为 $N$ 的非负整数序列 $A = (A_1, A_2, \ldots, A_N)$ 和 $B = (B_1, B_2, \ldots, B_N)$。

共有 $N$ 个袋子，编号为 $1$ 至 $N$。初始时，第 $i$ 个袋子中有 $A_i$ 枚金币和 $B_i$ 枚银币。

高桥君和青木君将使用这些袋子进行游戏。游戏开始时，高桥君选择若干袋子（可以不选），剩余未被选中的袋子归青木君所有。之后，两人轮流进行操作，高桥君先手：

- 从自己持有的袋子中选择一个包含至少 $1$ 枚金币或银币的袋子，并执行以下两种操作之一：
  - **移除 $1$ 枚金币**，并放入若干银币：若操作者为高桥君则放入 $X$ 枚，若为青木君则放入 $Y$ 枚（此操作仅在袋子中有至少 $1$ 枚金币时可执行）。
  - **移除 $1$ 枚银币**（此操作仅在袋子中有至少 $1$ 枚银币时可执行）。
- 操作完成后，将选中的袋子交给对方。

**无法进行任何操作的玩家判负**。

假设两人均采取最优策略，求高桥君能够获胜的初始选袋方案数（模 $998244353$ 后的结果）。

## 输入格式

输入通过标准输入给出，格式如下：

> $N$ $X$ $Y$  
> $A_1$ $B_1$  
> $A_2$ $B_2$  
> $\vdots$  
> $A_N$ $B_N$

## 输出格式

输出高桥君能够获胜的初始选袋方案数（模 $998244353$ 后的结果）。

## 输入输出样例 #1

### 输入 #1

```
2 1 1
1 0
1 1
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
2 2 1
1 2
1 2
```

### 输出 #2

```
3
```

## 输入输出样例 #3

### 输入 #3

```
5 8 3
0 0
0 0
0 0
0 0
0 0
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
7 2025 191
1323 9953
2763 3225
2624 5938
6718 2998
3741 7040
9837 1681
8817 4471
```

### 输出 #4

```
40
```

## 说明/提示

### 约束条件

- $1 \leq N \leq 2 \times 10^5$
- $1 \leq X, Y \leq 10^9$
- $0 \leq A_i, B_i \leq 10^9$
- 输入均为整数

### 样例解释 1

以高桥君初始选择袋子 $1$ 和 $2$ 的情况为例：
1. 高桥君从袋子 $2$ 移除 $1$ 枚金币，放入 $1$ 枚银币，并将袋子交给青木君。
2. 青木君从袋子 $2$ 移除 $1$ 枚银币，交还袋子。
3. 高桥君从袋子 $1$ 移除 $1$ 枚金币，放入 $1$ 枚银币，交出袋子。
4. 青木君从袋子 $1$ 移除 $1$ 枚银币，交还袋子。
5. 高桥君从袋子 $2$ 移除最后 $1$ 枚银币，青木君无法操作，高桥君获胜。

高桥君在初始选择袋子 $2$ 或同时选择袋子 $1$ 和 $2$ 时均可获胜，因此输出 $2$。

### 样例解释 2

高桥君初始选择袋子 $1$、$2$ 或两者时均可获胜。

### 样例解释 3

无论高桥君如何选择初始袋子，均无法获胜。

翻译由 DeepSeek R1 完成