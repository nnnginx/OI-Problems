## 题目描述

有一个长度很大的二进制串，初始时它的每一位都为 0。现在有 $m$ 个操作，其中第 $i$ 个操作是将这个二进制串的数值加上 ${2}^{a_i}$ $({0}\leq{a_i}\leq{n})$，或者说，给第 $a_i$ 位加上 $1$ 并进位，我们称每次操作的代价是这次操作改变的位的数量。例如，当前的二进制串是 $10111$ 时，如果给它加上 $2^0$，串就变成了 $11000$，其中从低到高第 $0,1,2,3$ 位发生了改变，那么这次操作代价为 $4$。

我们以一定概率执行这些操作：第 $i$ 个操作有 $p_i$ 的概率执行，否则不执行。请求出所有执行的操作的代价和的期望。

你只需要求出期望改变的位数在模 $998244353$ 意义下的值。具体来说，如果你算出来的期望$E = {\frac{P}{Q}}$，其中 $P,Q$ 互质，那么你只要输出 $({P}{Q^{-1}})\pmod{998244353}$，其中 $Q^{-1}\pmod{998244353}$ 表示 $Q$ 在 $\pmod{998244353}$ 意义下的逆元。

**注意：执行完操作后，该串去除前导 $0$ 后的长度可能大于 $n$。**

## 输入格式

第一行两个用空格分隔的正整数 $n,m$，分别表示 $a_i$ 的范围和操作数，如上文所述。

接下来 $m$ 行，每行三个正整数 $a_i, x_i, y_i$，其中 $p_i = {\frac{x_i}{y_i}}$。

## 输出格式

仅一行，表示答案。

```input1
4 4
0 1 2
0 1 2
0 1 2
0 1 2
```

```output1
187170819
```

```input2
233 6
1 166 233
2 233 666
3 166 266
4 233 266
5 233 666
6 166 233
```

```output2
56615945
```

## 数据范围与提示

对于所有数据，$1\le {n,m} \leq{200000}, 0\le x<998244353,1\le y<998244353$。

|子任务编号|分值|$n \leq$|$m\leq$|特殊限制|
|:------------:|:----:|:------------:|:--------:|:--------:|
|1|$5$|$17$|$17$|-|
|2|$15$|$1$|$3000$|$a_i=0$|
|3|$20$|$1$|$2\times 10^5$|$a_i=0$|
|4|$20$|$3000$|$3000$|-|
|5|$40$|$2\times 10^5$|$2\times 10^5$|-|


