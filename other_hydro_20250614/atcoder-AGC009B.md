分值：$800$ 分

## 题目描述

有 $N$ 名参赛者参加了一场比赛。总共进行了 $N-1$ 次淘汰赛。

由于某些原因，比赛可能对所有参赛者都不『公平』。也就是说，为了赢得冠军而必须进行的比赛的数量对于每个参赛者来说可能是不同的。淘汰赛的结构将在本声明的末尾进行正式描述。

每场比赛总有一个胜者和一个败者。最后剩下的那位参赛者将成为冠军。

![](https://atcoder.jp/img/agc009/783f7be9c88350e31963edba8a958879.png)

图：一个淘汰赛的例子

为了方便起见，参赛者被编号为 $1$ 到 $N$。编号为 $1$ 的选手是冠军，编号为 $i$（$2 \leq i\leq N$）的选手在与编号为 $a_i$ 的选手的比赛中被击败。

我们将比赛的『深度』定义为为了战胜所有参赛者赢得冠军而必须进行的最大比赛次数。

找出比赛可能的最小深度。

比赛的正式描述如下。在第 $i$ 场比赛中，下列选手中的一个相互对抗：

- 两名预先确定的参赛者；
- 一名预先确定的参赛者和第 $j$（$j < i$，$j$ 是预先确定的）场比赛的胜者；
- 第 $j$ 场和第 $j$ 场比赛（$j,k < i$，$j,k$ 是预先确定的）的胜者；

这是一种合法的比赛规划，前提是无论比赛结果如何，任何已经在比赛中被击败的选手都不会参加比赛。

## 数据范围

- $2 \leq N \leq 10^5$
- $1 \leq a_i \leq N$（$2 \leq i \leq N$）
- 保证输入合法（即至少存在一个符合条件的比赛）

## 输入格式

输入按照如下格式从标准输入给出：

> $N$
> 
> $a_2$
> 
> :
> 
> $a_N$

## 输出格式

输出比赛的最小可能深度。

```input1
5
1
1
2
4
```

```output1
3
```

The following tournament and the result of the matches are consistent with the given information:

- In the first match, contestants $4$ and $5$ played against each other, and contestant $4$ won.
- In the second match, contestants $2$ and $4$ played against each other, and contestant $2$ won.
- In the third match, contestants $1$ and $3$ played against each other, and contestant $1$ won.
- In the fourth match, contestants $1$ and $2$ played against each other, and contestant $1$ won.

![](https://atcoder.jp/img/agc009/783f7be9c88350e31963edba8a958879.png)

The depth of this tournament is $3$, since contestant $5$ must play three matches in order to win the championship.
There is no tournament with depth $2$ or less that is consistent with the given information, thus the output should be $3$.

```input2
7
1
2
1
3
1
4
```

```output2
3
```

```input3
4
4
4
1
```

```output3
3
```