## 题目描述
Farmer John has just arranged his $N$ haybales ($1 \leq N \leq 100,000$) at various points along the one-dimensional road running across his farm.  To make sure they are spaced out appropriately, please help him answer $Q$ queries ($1 \leq Q \leq 100,000$), each asking for the number of haybales within a specific interval along the road.

## 输入格式
The first line contains $N$ and $Q$.

The next line contains $N$ distinct integers, each in the range $0 \ldots 1,000,000,000$, indicating that there is a haybale at each of those locations.

Each of the next $Q$ lines contains two integers $A$ and $B$($0 \leq A \leq B \leq 1,000,000,000$) giving a query for the number of haybales between $A$ and $B$, inclusive.

## 输出格式
You should write $Q$ lines of output.  For each query, output the number of haybales in its respective interval.

## 题目大意
### 题目描述

Farmer John 刚刚将他的 $N$ 个干草捆（$1 \leq N \leq 100,000$）安排在他农场的一维道路上的各个位置。为了确保它们之间的间距合适，请帮助他回答 $Q$ 个查询（$1 \leq Q \leq 100,000$），每个查询询问在道路的特定区间内有多少个干草捆。

### 输入格式

第一行包含 $N$ 和 $Q$。

第二行包含 $N$ 个不同的整数，每个整数的范围在 $0 \ldots 1,000,000,000$ 之间，表示每个位置上有一个干草捆。

接下来的 $Q$ 行每行包含两个整数 $A$ 和 $B$（$0 \leq A \leq B \leq 1,000,000,000$），表示一个查询，询问在 $A$ 到 $B$（包括 $A$ 和 $B$）的区间内有多少个干草捆。

### 输出格式

你需要输出 $Q$ 行。对于每个查询，输出其对应区间内的干草捆数量。

```input1
4 6
3 2 7 5
2 3
2 4
2 5
2 7
4 6
8 10
```

```output1
2
2
3
4
1
0
```

