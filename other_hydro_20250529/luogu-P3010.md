## 题目描述
Bessie and Canmuu found a sack of N (1 <= N <= 250) gold coins that they wish to divide as evenly as possible. Coin i has value v\_i (1 <= V\_i <= 2,000). The cows would like to split the pile as evenly as they can, but that is not always possible. What is the smallest difference between the values of the two piles?

In addition, the Bessie and Canmuu have found that there might be multiple ways to split the piles with that minimum difference. They would also like to know the number of ways to split the coins as fairly as possible. If it isn't possible to split the piles evenly, Bessie will get the higher-valued pile.

By way of example, consider a sack of five coins of values: 2, 1, 8, 4, and 16. Bessie and Canmuu split the coins into two piles, one pile with one coin worth 16, and the other pile with the remaining coins worth 1+2+4+8=15. Therefore the difference is 16-15 = 1.  This is the only way for them to split the coins this way, so the number of ways to split it evenly is just 1.

Note that same-valued coins can be switched among the piles to increase the number of ways to perform an optimal split. Thus, the set of coins {1, 1, 1, 1} has six different ways to split into two optimal partitions, each with two coins.

## 输入格式
\* Line 1: A single integer: N

\* Lines 2..N+1: Line i+1 contains a single integer: V\_i


## 输出格式
\* Line 1: A single integer that is the smallest difference of two partitions.

\* Line 2: A single integer that is the number of ways to split the coins with the minimum difference printed in line 1. Since this number can get quite large, print the remainder when divided by 1,000,000.


## 题目大意
Bessie 和 Canmuu 发现了一个有 ***N*** 个金币的袋子(1 <= N <= 250) 。第i个金币有一个价值 ***Vi***
(1 <= Vi <= 2000)他们希望尽可能的把这堆金币平均分配，但有时这是不可能的。找出使两堆价值差最小的分配方案。如果不能完全平均分开，Bessie会获得较高价值那一堆。

举例来说 ： 有一袋5个金币。价值分别是 2,1,8,4,16。
Bessie 和Canmuu把金币分成两堆，第一堆是价值16的金币，另一堆是剩下的1+2+4+8 = 15 个金币，因此，差是1，这是最优分配方案下的唯一分法（即差最小的唯一分法），所以方案数为1。


请你找出 **最小的差值** 以及在这个差值下分配的**方案数。**

输入第一行 N

之后每一行有一个Vi代表第i个金币的价值

输出第一行是最小差值，

第二行是分配方案数 ,由于方案数可能很大，输出***ans mod 1e6***的答案

感谢@ToBiChi 提供翻译

```input1
5 
2 
1 
8 
4 
16 

```

```output1
1 
1 

```

