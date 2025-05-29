## 题目描述

给出 $n$ 个结点以及每个点初始时对应的权值 $w_i$。起始时点与点之间没有连边。有3类操作：

1. `bridge A B`：询问结点 $A$ 与结点 $B$ 是否连通。如果是则输出 `no`。否则输出`yes`，并且在结点 $A$ 和结点 $B$ 之间连一条无向边；
2. `penguins A X`：将结点 $A$ 对应的权值 $w_A$ 修改为 $X$；
3. `excursion A B`：如果结点 $A$ 和结点 $B$ 不连通，则输出 `impossible`。否则输出结点 $A$ 到结点 $B$ 的路径上的点对应的权值的和。

给出 $q$ 个操作，要求在线处理所有操作。

## 输入格式


第一行包含一个整数 $n$，表示节点的数目。

第二行包含 $n$ 个整数，第 $i$ 个整数表示第 $i$ 个节点初始时对应的权值。

第三行包含一个整数 $q$，表示操作的数目。

以下 $q$ 行，每行包含一个操作，操作的类别见题目描述。

## 输出格式


输出所有 `bridge` 操作和 `excursion` 操作对应的输出，每个一行。

```input1
5
4 2 4 5 6
10
excursion 1 1
excursion 1 2
bridge 1 2
excursion 1 2
bridge 3 4
bridge 3 5
excursion 4 5
bridge 1 3
excursion 2 4
excursion 2 5
```

```output1
4
impossible
yes6
yes
yes
15
yes
15
16
```

## 数据规模与约定


对于 $100\%$ 的数据，$1\le n\le 3\times 10^4$，$1\le q\le 3\times 10^5$，$0\le w_i\le 1000$。

任意时刻每个节点对应的权值都是 $1$ 到 $1000$ 的整数。