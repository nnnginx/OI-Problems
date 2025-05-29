## 题目描述

这是一道模板题。

给出一个非负整数 $k$ 和正整数 $m$，求 Eulerian 数

$$
\left\langle 0\atop k\right\rangle,\left\langle 1\atop k\right\rangle,\dots ,\left\langle {m-1}\atop k\right\rangle
$$

在模 $p=998244353$ 下的答案。

其中 $\left\langle n\atop k\right\rangle =\sum_{j=0}^k(-1)^j\binom{n+1}{j}(k-j+1)^n$。

## 输入格式

一行两个整数 $k,m$。

## 输出格式

一行 $m$ 个整数分别为 $\left\langle 0\atop k\right\rangle \bmod{p},\left\langle 1\atop k\right\rangle \bmod{p},\dots ,\left\langle {m-1}\atop k\right\rangle \bmod{p}$。

```input1
0 10
```

```output1
1 1 1 1 1 1 1 1 1 1
```



$\left\langle n\atop 0\right\rangle =1,\forall n\geq 0$。

```input2
3 10
```

```output2
0 0 0 0 1 26 302 2416 15619 88234
```

## 数据范围与提示

本题包含 $4$ 个子任务，每个子任务 $25$ 分，第 $n$ 个子任务满足 $0\leq k\leq 10^{n+1},1\leq m\leq 10^{n+1}$。

