## 题目背景
一天 zzq 没有题可以出了。于是他随便写了一个式子，求$\sum_{i=0}^n \sum_{j=0}^m i \operatorname{xor}j\operatorname{xor}x$，其中 $\operatorname{xor}$ 表示异或。

zzy 一看，这不是水题吗，就随便加了一个函数：$\sum_{i=0}^n \sum_{j=0}^m d(i \operatorname{xor}j\operatorname{xor}x)$，其中 $\operatorname{xor}$ 表示异或，$d(x)$ 表示 $x$ 的约数个数。**注意 $d(0)=0$。**

现在 zzq 不会做了，只好写了一个暴力造了数据，然后把这道题丢给了你。


## 题目描述
输入三个数 $n,m,x$，要求计算 $\sum_{i=0}^n \sum_{j=0}^m d(i \operatorname{xor}j\operatorname{xor}x)$，其中 $\operatorname{xor}$ 表示二进制下的异或，$d(x)$ 表示 $x$ 的约数个数。

由于答案比较大，要求输出答案模 $ 998244353$ 后的结果。


## 输入格式
一行三个数 $n,m,x$。


## 输出格式
输出答案模 $ 998244353$ 后的结果。

```input1
0 2 233
```

```output1
14
```

```input2
123 234 345
```

```output2
205761
```

## 提示
对于 $20\%$ 的数据，$n,m,x \leq 2000$。

对于 $50\%$ 的数据，$n,m,x \leq 10^6$。

对于 $80\%$ 的数据，$n,m,x \leq 10^8$。

对于 $100\%$ 的数据，$1 \leq n,m,x \leq 10^{10}$。


