## 题目描述

首先知道 $A \operatorname{nand} B=\operatorname{not} (A \operatorname{and} B)$ （运算操作限制了数位位数为 $k$）比如 $2 \operatorname{nand} 3,k=3$，则 $2 \operatorname{nand} 3=\operatorname{not} (2 \operatorname{and} 3)=\operatorname{not} 2=5$。

给出一棵树，树上每个点都有点权，定义树上从 $a$ 到 $b$ 的费用为 $0$ 与路径上的点的权值顺次 $\operatorname{nand}$ 的结果，例如：从 $2$ 号点到 $5$ 号点顺次经过 $2\to 3\to 5$，权值分别为 $5,7,2,k=3$，那么最终结果为 $0 \operatorname{nand} 5 \operatorname{nand} 7 \operatorname{nand} 2=7 \operatorname{nand} 7 \operatorname{nand} 2=0 \operatorname{nand} 2=7$，现在这棵树需要支持以下操作。

1. `Replace a b`：将点 $a$（$1\le a\le n$）的权值改为 $b$。
2. `Query a b`：输出点 $a$ 到点 $b$ 的费用。

请众神给出一个程序支持这些操作。

## 输入格式

- 第一行 $n,m,k$，树的节点数量、总操作个数和运算位数。
- 接下来一行 $n$ 个数字，依次表示节点 $i$ 的权值。
- 接下来 $n-1$ 行，每行两个数字 $a,b$（$1\le a,b\le n$）表示 $a,b$ 间有一条树边。
- 接下来 $m$ 行，每行一个操作，为以上 $2$ 类操作之一。

## 输出格式

- 对于操作 $2$ 每个输出一行，如题目所述。

```input1
3 3 3
2 7 3 
1 2
2 3
Query 2 3
Replace 1 3
Query 1 1
```

```output1
4
7
```

## 数据规模与约定

对于 $100\%$ 的数据，$n,m\le 10^5$，$k\le 32$。

