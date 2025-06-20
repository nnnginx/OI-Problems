# AT_arc038_d [ARC038D] 有向グラフと数

## 题目描述

有一有向图，带有 $N$ 个顶点和 $M$ 条边。图中的每个顶点上都写有整数，第 $i$ 个顶点上的整数是 $X_{i}$ 。一对喜欢玩游戏的兄妹用一枚象棋“马”在上面玩游戏。

- 游戏开始时，马位于 $1$ 号顶点。
- 在自己的回合，玩家必须在下述操作中恰好选择一项：
	+ **移动**：将马沿着边，从其当前所在的顶点移动至相邻顶点。必须恰好移动 $1$ 次；
    + **结束**：使游戏结束。
- 两名玩家轮流进入自己的回合。当有玩家执行“结束”操作时、或者在后手恰好移动 $10^{9}$ 次后，游戏立即结束。此时，游戏的**分数**就是马所在的顶点上写着的整数。

先手会采取行动使得分数尽可能地大，后手会采取行动使得分数尽可能地小。你知道游戏分数最后会是多少吗？

## 输入格式

输入数据以下述格式从标准输入给出。

- 第一行中的两个整数 $N$ 和 $M$ 分别表示图的顶点数和边数，以空格分隔。其中，$1 \le N \le 100,000$，$1 \le M \le 200,000$；
- 第二行中的 $N$ 个整数，依次对应各顶点上写着的整数，以空格分隔。其中，第 $i$ 个整数 $X_{i} $对应 $i$ 号顶点，$1\le i\le N$，$0 \le X_{i} \le 10^{9}$；
- 从第三行起，包括第三行在内的 $M$ 行，每一行给出以空格分隔的两个整数 $A_{i}$，$B_{i}$ ，表示从顶点  $A_{i}$ 到顶点 $B_{i}$  存在一条有向边，其中，$1 \le i \le M,$$1\le A_{i}\le N,$$1\le B_{i}\le N,$$A_{i} \neq B_{i}$。输入数据中不含有相同的边，即，当$p \neq q$ 时，$A_{p} \neq A_{q}$ 或者 $B_{p} \neq B_{q}$ 成立。

## 输出格式

一行，输出游戏的分数，行末输出换行符。

## 输入输出样例 #1

### 输入 #1

```
3 3
1 3 2
1 2
2 3
3 1
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
4 5
1 3 2 1
1 2
2 3
3 1
2 4
4 3
```

### 输出 #2

```
1
```

## 说明/提示

## 分部计分
此题分部计分。
- 数据集 $1$ 满足 $N \le 1000,$$M \le 2000$，解答正确者计 $30$ 分；
- 全部正确者，在上述 $30$ 分的基础上再计 $70$ 分。

此例中，游戏以下述过程进行：
- 先手将马从顶点 1 移至顶点 2 ；
- 后手将马从顶点 2 移至顶点 3 ；
- 先手结束游戏。

此时游戏结束，分数为2。在后手采取最优策略的情况下，先手不论采取何种策略，都不可能使分数大于2；且，在先手采取最优策略的情况下，后手不论采取何种策略，都不可能使分数小于2。

此例中，游戏以下述过程进行：
- 先手将马从顶点 1 移至顶点 2 ；
- 后手将马从顶点 2 移至顶点 4 ；
- 先手将马从顶点 4 移至顶点 3 ；
- 后手将马从顶点 3 移至顶点 1 ；
- （上述过程重复）
- 后手的第 $10^{9}$ 次移动，将马从顶点 3 移至顶点 1。

此时游戏结束，分数为1。在后手采取最优策略的情况下，先手不论采取何种策略，都不可能使分数大于1；且，在先手采取最优策略的情况下，后手不论采取何种策略，都不可能使分数小于1。