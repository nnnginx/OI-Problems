# AT_joisc2014_f 友だちをつくろう

## 题目描述

你是活跃在历史幕后的一名特工，为了世界和平而夜以继日地努力着。

这个世界有 $N$ 个国家，编号为 $1…N$，你的目的是在这 $N$ 个国家之间建立尽可能多的友好关系。你为了制定一个特工工作的计划，作出了一张当今国际关系的示意图。
你准备了一张非常大的画纸，先画下了代表每个国家的 $N$ 个点。接下来，为了表示现在的国际关系，画下了 $M$ 个连接两个国家的有向边，其中从国家 $a$ 连向国家 $b$ 的有向边，表示「现在国家 $a$ 向国家 $b$ 派遣了大使」，下文称作边 $(a,b)$。这样就做出了 $N$ 个点 $M$ 条边的当今国际关系示意图。

作为两国友好关系的开端，两国之间需要进行「友好条约缔结会议」，以下简称会议。如果某两个国家 $p$ 和 $q$ 要进行会议，那么需要一个向两国都派遣了大使的国家 $x$ 作为中介。会议结束后，会议的双方相互向对方的国家派遣大使。换句话说，为了让国家 $p$ 和国家 $q$ 进行会议，必须存在一个国家 $x$ 满足边 $(x,p)$ 和边 $(x,q)$ 都存在，并且在会议后添加两条边 $(p,q)$ 和 $(q,p)$（如果需要添加的某条边已经存在则不添加）。

你的工作是对于可以进行会议的两国，选择会议的中介并促使会议进行。使用这张图进行工作的模拟的话，世界距离和平还有多远的一个重要的基准就是这张图上的边数。

现在给出国家的个数以及当今国际关系的情报，请你求出反复「选择两个国家，促使它们其进行会议」后，图上最多会有多少条边。

## 输入格式

第一行两个空格分隔的整数 $N$ 和 $M$，分别表示世界上国家的个数和图中的边数。

接下来 $M$ 行描述画纸上的有向边的信息，其中第 $i$ 行有两个空格分隔的整数 $A_i$ 和 $B_i$，表示图中有一条从 $A_i$ 到 $B_i$ 的有向边。

## 输出格式

输出一行一个整数，表示能实现的边数的最大值。注意这个边数包括原有的边数和新连接的边数。

## 输入输出样例

### 样例输入 #1

```
5 4
1 2
1 3
4 3
4 5
```

### 样例输出 #1

```
10
```

## 说明/提示

【样例解释 1】

国家 $1$ 作为中介国，国家 $2$ 与 $3$ 开会。

国家 $4$ 作为中介国，国家 $3$ 与 $5$ 开会。

国家 $3$ 作为中介国，国家 $2$ 与 $5$ 开会。

因此最多的边数就是 $4+6=10$ 条。


对于 $100\%$ 的数据，$1≤N≤10^5,1≤M≤2\times 10^5,1≤A_i,B_i≤N,A_i≠B_i,(A_i,B_i)≠(A_j,B_j)$。