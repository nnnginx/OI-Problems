## 题目描述
The cows are building a roller coaster! They want your help to design as fun a roller coaster as possible, while keeping to the budget.

The roller coaster will be built on a long linear stretch of land of length L (1 ≤ L ≤ 1,000). The roller coaster comprises a collection of some of the N (1 ≤ N ≤ 10,000) different interchangable components. Each component i has a fixed length Wi (1 ≤ Wi ≤ L). Due to varying terrain, each component i can be only built starting at location Xi (0 ≤ Xi ≤ L - Wi). The cows want to string together various roller coaster components starting at 0 and ending at L so that the end of each component (except the last) is the start of the next component.

Each component i has a "fun rating" Fi (1 ≤ Fi ≤ 1,000,000) and a cost Ci (1 ≤ Ci ≤ 1000). The total fun of the roller coster is the sum of the fun from each component used; the total cost is likewise the sum of the costs of each component used. The cows' total budget is B (1 ≤ B ≤ 1000). Help the cows determine the most fun roller coaster that they can build with their budget.

## 输入格式
Line 1: Three space-separated integers: L, N and B.


Lines 2..N+1: Line i+1 contains four space-separated integers, respectively: Xi, Wi, Fi, and Ci.


## 输出格式
Line 1: A single integer that is the maximum fun value that a roller-coaster can have while staying within the budget and meeting all the other constraints. If it is not possible to build a roller-coaster within budget, output -1.


## 题目大意
**【题目描述】**

有 $n$ 条线段，每条线段只能放在数轴上的一个特定位置，并且第 $i$ 根线段有如下几个属性：$X_i$（该线段放在数轴上的起点），$W_i$（该线段长度），$F_i$（你若使用该线段你能获得的价值），$C_i$（你若使用该线段你所需要的费用）。现在让你从中选出一些线段，使得这些线段能够铺满数轴上的区间 $[0,L]$ 且线段必须首尾相接（也就是不能重叠，也不能空缺），并且所花费用和不超过 $B$，同时要使你收获的价值尽量大，请你找到这个方案。

**【输入格式】**

第一行三个整数 $L, n, B$。

接下来 $n$ 行，每行四个整数 $X_i, W_i, F_i, C_i$ 表示第 $i$ 根线段的四个属性。

**【输出格式】**

一个整数，表示你能获得的最大价值和。若无法满足上述要求，则输出 $-1$。

```input1
5 6 10
0 2 20 6
2 3 5 6
0 1 2 1
1 1 1 3
1 2 5 4
3 2 10 2
```

```output1
17
```

## 提示
Taking the 3rd, 5th and 6th components gives a connected roller-coaster with fun value 17 and cost 7. Taking the first two components would give a more fun roller-coaster (25) but would be over budget.


