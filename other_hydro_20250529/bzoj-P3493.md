## 题面描述

有两个玩家，会去挑选一些数字，每次只能选至少与一个 $0$ 相邻的数字（不能选 $0$），拿完一个数字后这个数字会变成 $0$。

两个玩家都采取最优策略，使自己拿到的数字的和最大，问最后两位玩家的得分。

## 输入格式

第一行一个正整数 $n$, 表示数字的数量

第二行 $n$ 个整数, 为给定的数字

## 输出格式

两个整数, 分别为最后两位玩家的得分.

## 样例输入

```
8
1 2 0 3 7 4 0 9
```

## 样例输出

```
17 9
```

## 样例解释

Explanation of the example: The fence consisted of 8 planks, out of which 2 have already been eaten. The first termite in his first turn can choose between planks of heights 2, 3, 4 and 9. During the optimal game, in the consecutive turns, termites will eat planks of heights 9, 2, 1, 4, 7 and 3.

## 数据范围

对于所有的数据, 满足 $n < 10^6$. 保证初始时至少有一个 $0$.