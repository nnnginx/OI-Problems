## 题目描述

Maishroom 拿到了一张 $n\times m$ 的数表，其中左上角的数是 $0$，其他数都在 $[0,s]$ 中。

Maishroom 想从左上角走到右下角，每一步只能向下或向右走，使得路径上数之和最大。

这是个有趣的题目，因为有一个正确性显然不对的贪心算法，伪代码如下：

```
Greedily_Act(Now_n, Now_m)
If Now_m == M
    MOVE_DOWN
Else If Now_n == N
    MOVE_RIGHT
Else If V[Now_n][Now_m + 1] >= V[Now_n + 1][Now_m]
    MOVE_RIGHT
Else
    MOVE_DOWN
End
```

Maishroom 知道你们用脚趾头都能做出原来那道题，

于是现在他的问题是：求出有多少种数表，满足在该贪心算法下的答案为 $s$。

## 输入格式

一行四个整数 $n,m,s,p$。

## 输出格式

一行一个整数，表示答案对 $p$ 取模的结果。

```input1
2 2 2 1000000007
```

```output1
9
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n,m,s\leq 10^6$，$10^8\leq p\leq 2^{30}$，保证 $p$ 是质数。

