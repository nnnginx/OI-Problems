## 题目描述

有 $n$ 个机器，每个机器有 $2$ 个芯片，每个芯片可以放 $k$ 个电池。

每个芯片能量是 $k$ 个电池的能量的最小值。

两个芯片的能量之差越小，这个机器就工作的越好。

现在有 $2nk$ 个电池，已知它们的能量，我们要把它们放在 $n$ 个机器上的芯片上，

使得所有机器的能量之差的最大值最小。

## 输入格式

第一行，两个正整数，$n,k$。

第二行，$2nk$ 个整数，表示每个电池的能量 $p_i$。

## 输出格式

一行一个整数，表示所有机器的能量之差的最大值最小是多少。

```input1
2 3
1 2 3 4 5 6 7 8 9 10 11 12
```

```output1
1
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq 2nk\leq 10^6$，$1\leq p_i\leq 10^9$。

