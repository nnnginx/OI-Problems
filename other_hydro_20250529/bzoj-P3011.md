## 题目描述

It's milking time at Farmer John's farm, but the cows have all run away! Farmer John needs to round them all up, and needs your help in the search. FJ's farm is a series of  $ N $  pastures numbered  $ 1...N $  connected by  $ N - 1 $  bidirectional paths. The barn is located at pasture  $ 1 $ , and it is possible to reach any pasture from the barn. FJ's cows were in their pastures this morning, but who knows where they ran to by now. FJ does know that the cows only run away from the barn, and they are too lazy to run a distance of more than  $ L $ .

For every pasture, FJ wants to know how many different pastures cows starting in that pasture could have ended up in. Note: 64-bit integers (int64 in Pascal, long long in C/C++ and long in Java) are needed to store the distance values.

题目大意：给出以 $ 1 $ 号点为根的一棵有根树，问每个点的子树中与它距离小于 $ L $ 的点有多少个。

## 输入格式

Line 1: 2 integers,  $ N $  and  $ L $.

Lines 2..N: The ith line contains two integers  $ p_i $  and  $ l_i $. $ p_i (1 \leq p_i < i) $  is the first pasture on the shortest path between pasture  $ i $  and the barn, and  $ l_i (1 \leq l_i \leq 10^{12}) $  is the length of that path.

## 输出格式

Lines 1..N: One number per line, the number on line  $ i $  is the number pastures that can be reached from pasture  $ i $  by taking roads that lead strictly farther away from the barn (pasture  $ 1 $ ) whose total length does not exceed  $ L $.

## 样例输入

```
4 5
1 4
2 3
1 5
```

## 样例输出

```
3
2
1
1
```

## 提示

OUTPUT DETAILS: Cows from pasture  $ 1 $  can hide at pastures  $ 1, 2 $  and  $ 4 $. Cows from pasture  $ 2 $  can hide at pastures  $ 2 $  and  $ 3 $ . Pasture  $ 3 $  and  $ 4 $  are as far from the barn as possible, and the cows can hide there.

## 数据规模与约定

对于 $100\%$ 的数据， $ 1 \leq N \leq 2\times 10^5 $ ， $ 1 \leq L \leq 10^{18} $

