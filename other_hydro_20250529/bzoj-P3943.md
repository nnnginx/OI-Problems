## 题目描述

贝西和她的朋友们在参加一年一度的「犇」（足）球锦标赛。FJ 的任务是让这场锦标赛尽可能地好看。

一共有 $N$ 支球队参加这场比赛，每支球队都有一个特有的整数编号（即：所有球队编号各不相同）。「犇」锦标赛是一个淘汰赛制的比赛——每场比赛过后，FJ 选择一支球队淘汰，淘汰了的球队将不能再参加比赛。锦标赛在只有一支球队留下的时候就结束了。

FJ 发现了一个神奇的规律：在任意一场比赛中，这场比赛的得分是参加比赛两队的编号的异或（xor）值。例如：编号为 $12$ 的队伍和编号为 $20$ 的队伍之间的比赛的得分是 $24$ 分，因为 $12(01100)\text{ xor }20(10100) = 24(11000)$。FJ 相信比赛的得分越高，比赛就越好看，因此，他希望安排一个比赛顺序，使得所有比赛的得分和最高。请帮助 FJ 决定比赛的顺序。

## 输入格式

第一行包含一个整数 $N$。

接下来的 $N$ 行包含 $N$ 个整数，第 $i$ 个整数代表第 $i$ 支队伍的编号。

## 输出格式

一行，一个整数，表示锦标赛的所有比赛的得分的最大值。

```input1
4
3
6
9
10
```

```output1
37
```

## 样例解释

FJ 先让编号为 $3$ 和编号为 $9$ 的队伍进行比赛，然后让编号为 $9$ 的队伍赢得比赛（淘汰编号为 $3$ 的队伍），现在
剩下了编号为 $6,9,10$ 的队伍。

然后他让编号为 $6$ 和编号为 $9$ 的队伍比赛，然后让编号为 $6$ 的队伍赢得比赛。现在编号为 $6,10$ 的队伍留了下来。

最后让编号为 $6$ 和编号为 $10$ 的队伍比赛，让编号为 $10$ 的队伍赢得比赛。所有比赛的得分和就是：$(3\text{ xor }9)+(6\text{ xor }9)+(6\text{ xor }10)=10+15+12=37$。

## 数据范围与提示

对于 $100\%$ 的数据，$1\le N\le 2000$，且编号 $x$ 满足 $1\le x\le 2^{30}-1$。

## 题目来源

[USACO February 2015 Contest](http://www.usaco.org/index.php?page=feb15results) Silver T3