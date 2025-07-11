# AT_joi2008yo_f 船旅

## 题目描述

在 JOI 国，有 $n$ 个岛屿，每个岛屿都有一个从 $1$ 到 $n$ 的编号。这个国家正在积极开展岛屿之间的航线建设。

你在一家船票售卖中心工作。许多客户希望通过船只在岛屿之间用最低的费用旅行，并把他们的出发地和目的地写在订单上交给你。

你的任务是，接到客户的订单后，立即计算出可以从出发地到达目的地的最低票价，并将结果告知客户。

注意，有些行程可能无法通过船只到达，如果是这种情况，你需要告诉客户「无法通过船只旅行」。同时，JOI 国不断有新航线开通，相关信息会实时传递给你，因此你需要根据最新的信息进行回复。

请编写一个程序，根据输入的客户订单和新航线信息，给出每个订单的回复。

## 输入格式

第一行输入两个整数 $n, k$ ($1 \leq n \leq 100$，$1 \leq k \leq 5000$)，表示有 $n$ 个岛屿，输入共 $k + 1$ 行。

接下来的 $k$ 行每行包含 3 或 4 个整数，用空格分隔：

- 若第一个数字为 0，代表客户订单。
  这一行有 3 个整数 $0, a, b$ ($1 \leq a \leq n$，$1 \leq b \leq n$ 且 $a \neq b$)，表示客户希望从岛屿 $a$ 前往岛屿 $b$。

- 若第一个数字为 1，代表新开通的航线信息。
  这一行有 4 个整数 $1, c, d, e$ ($1 \leq c \leq n$，$1 \leq d \leq n$ 且 $c \neq d$，$1 \leq e \leq 1,000,000$)，表示岛屿 $c$ 和岛屿 $d$ 之间有一条新航线，其票价为 $e$，且从 $c$ 到 $d$ 和从 $d$ 到 $c$ 的票价相同。在此之后的订单需要考虑这条新航线。

初始时，所有岛屿之间没有航线。输入中用于表示航线的信息行不超过 1000 行。此外，某些岛屿之间可能会有多条航线。

## 输出格式

假定输入中表示客户订单的行数为 $m$。输出应包含 $m$ 行，第 $i$ 行 ($1 \leq i \leq m$) 是对第 $i$ 个订单的回复：

- 如果可以从订单的出发地通过一些船只中转到达目的地，则输出最低的总票价；
- 如果无法通过船只从出发地到目的地，则输出 $-1$。

 **本翻译由 AI 自动生成**

## 输入输出样例 #1

### 输入 #1

```
3 8
1 3 1 10
0 2 3
1 2 3 20
1 1 2 5
0 3 2
1 1 3 7
1 2 1 9
0 2 3
```

### 输出 #1

```
-1
15
12
```

## 输入输出样例 #2

### 输入 #2

```
5 16
1 1 2 343750
1 1 3 3343
1 1 4 347392
1 1 5 5497
1 2 3 123394
1 2 4 545492
1 2 5 458
1 3 4 343983
1 3 5 843468
1 4 5 15934
0 2 1
0 4 1
0 3 2
0 4 2
0 4 3
0 5 3
```

### 输出 #2

```
5955
21431
9298
16392
24774
8840
```