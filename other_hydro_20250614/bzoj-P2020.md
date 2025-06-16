## 题目描述

Farmer John needs to travel to town to pick up $k$ pounds of feed. Driving $D$ miles with $k$ pounds of feed in his truck costs $d \times k$ cents. The county feed lot has $n$ stores (conveniently numbered $1\ldots n$) that sell feed. Each store is located on a segment of the $x$ axis whose length is $e$. Store $i$ is at location $x_i$ on the number line and can sell FJ as much as $f_i$ pounds of feed at a cost of $c_i$ cents per pound. Amazingly, a given point on the $x$ axis might have more than one store. FJ starts at location $0$ on this number line and can drive only in the positive direction, ultimately arriving at location $e$, with at least $k$ pounds of feed. He can stop at any of the feed stores along the way and buy any amount of feed up to the the store's limit. What is the minimum amount FJ has to pay to buy and transport the $k$ pounds of feed? FJ knows there is a solution. Consider a sample where FJ needs two pounds of feed from three stores (locations: $1,3,4$) on a number line whose range is $0 \ldots 5$:

```plain
0   1   2   3   4   5
+---|---+---|---|---+
    1       1   1      Available pounds of feed
    1       2   2      Cents per pound
```

It is best for FJ to buy one pound of feed from both the second and third stores. He must pay two cents to buy each pound of feed for a total cost of $4$. When FJ travels from $3$ to $4$ he is moving $1$ unit of length and he has $1$ pound of feed so he must pay $1 \times 1 = 1$ cents. When FJ travels from $4$ to $5$ he is moving one unit and he has $2$ pounds of feed so he must pay $1 \times 2 = 2$ cents. The total cost is $4+1+2 = 7$ cents.

FJ 开车去买 $k$ 份食物，如果他的车上有 $x$ 份食物。每走一里就花费 $x$ 元。FJ 的城市是一条线，总共 $e$ 里路，有 $e+1$ 个地方，标号 $0\sim 5$。FJ 从 $0$ 开始走，到 $e$ 结束（不能往回走），要买 $k$ 份食物。城里有 $n$ 个商店，每个商店的位置是 $x_i$（一个点上可能有多个商店），有 $f_i$ 份食物，每份 $c_i$ 元。问到达 $e$ 并买 $k$ 份食物的最小花费。

## 输入格式

第一行：$k,e,n$。  

第二行到第 $n+1$ 行：$x_i,f_i,c_i$。

## 输出格式

没有写明输出格式。

```input1
2 5 3
3 1 2
4 1 2
1 1 1
```
```output1
7
```

## 样例说明 1

在离家较近的两家商店里各购买一吨饲料，则花在路上的钱是 $1+2=3$，花在店里的钱是 $2+2=4$。

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq k\leq 100$，$1\leq f_i\leq 100$，$1\leq n\leq100$，$1\leq e\leq350$，$0 < x_i < e$，$1\leq c_i\leq 10^6$。

## 题目来源

Silver