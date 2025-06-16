## 题目背景
译自 [PA 2014](https://sio2.mimuw.edu.pl/c/pa-2014-1/p/) R5。


## 题目描述
给定 $k$ 个长度为 $n$ 的序列 $A_1,A_2,\cdots,A_k$。

定义两个长度为 $n$ 的序列 $a,b$ 的**距离** $\operatorname{dist}(a,b)$ 为：

$$\operatorname{dist}(a,b)=\sum_{1\le i\le n} |a_i-b_i|$$

你需要构造一个长度为 $n$ 的序列 $B$，最小化 $\displaystyle \max_{1\le i\le k} \operatorname{dist}(A_i,B)$ 的值。


## 输入格式
第一行，两个正整数 $n,k$。

接下来 $k$ 行，第 $i$ 行 $n$ 个整数 $A_{i,1},A_{i,2},\cdots,A_{i,n}$。

## 输出格式
输出 $n$ 个整数，表示你构造的 $B$ 序列。

**你需要保证**你输出的数在 $[-2^{31},2^{31})$ 内。


```input1
5 3
1 -1 2 -1 2
1 2 2 1 2
2 2 -1 1 1
```

```output1
1 2 2 1 2
```

## 提示
- $2\le n\le 10^5$；
- $2\le k\le 5$；
- $|A_{i,j}|\le 10^9$。

