## 题目描述

我们的小朋友很喜欢计算机科学，而且尤其喜欢二叉树。

考虑一个含有 $n$ 个互异正整数的序列 $c_1,c_2,\cdots,c_n$。如果一棵带点权的有根二叉树满足其所有顶点的权值都在集合 $\left\{c_1,c_2,\cdots,c_n\right\}$ 中，我们的小朋友就会将其称作神犇的。并且他认为，一棵带点权的树的权值，是其所有顶点权值的总和。

给出一个整数 $m$，你能对于任意的 $s$（$1\le s\le m$）计算出权值为 $s$ 的神犇二叉树的个数吗？请参照样例以更好的理解什么样的两棵二叉树会被视为不同的。

我们只需要知道答案关于 $998244353$（$7*17*2^{23}+1$，一个质数）取模后的值。

## 输入格式

第一行有两个整数 $n,m$。

第二行有 $n$ 个用空格隔开的互异的整数 $c_1,c_2,\cdots,c_n$。


## 输出格式

输出 $m$ 行，每行有一个整数。第 $i$ 行应当含有权值恰为 $i$ 的神犇二叉树的总数。请输出答案关于       $998244353$（$7*17*2^{23}+1$，一个质数）取模后的结果。



```input1
2 3
1 2
```
```output1
1
3
9
```

```input2
3 10
9 4 3
```
```output2
0
0
1
1
0
2
4
2
6
15
```

```input3
13 10 6 4 15
5 10
```
```output3
0
0
0
1
0
1
0
2
0
5
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\le n\le 10^5$，$1\le m\le 10^5$，$1\le c_i\le 10^5$。

## 样例解释

对于第一个样例，有 $9$ 个权值恰好为 $3$ 的神犇二叉树：

![](./3175/file/pic1.jpg)

## 题目来源

`VFleaKing & pyx1997 感谢 wyl8899 提供中文翻译。`

