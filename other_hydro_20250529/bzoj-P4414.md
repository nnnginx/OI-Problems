

## 题目描述
神犇 heheda 最近得到了 UOJ 抱枕，蒟蒻 yts1999 想要玩。于是 heheda 给 yts1999 出了一道题：

一个长度为 $2n+2$ 的整数数列，按照下式定义：

$$
A_0=0\\
A_1=C\\
A_{i+2}=(A_{i+1}+A_i) \bmod M
$$

现有 $n$ 个平面向量 $v_1\dots v_n$：

$$
V_1=(A_2,A_3)\\
V_2=(A_4,A_5)\\
\dots\\
V_n=(A_{2n},A_{2n+1})
$$

集合 $S$ 的定义如下：

$$
S=\{(v_i\cdot v_j \bmod M|1\le i,j\le n,i\ne j)\}
$$

其中"$v_i\cdot v_j$"表示向量 $v_i$ 和 $v_j$ 的数量积。

求 $S$ 集合中不同元素对 $M$ 取模的个数是多少。

heheda 告诉 yts1999，只要他做出了这道题，她就可以把抱枕借给他玩一会。然而 yts1999 实在是太弱了不会做，于是向你求助。

## 输入格式
输入数据包含一行三个整数 $C,M,n$，分别表示 $A_1$ 的值，模数和平面向量的个数，每两个数之间用一个空格隔开。

## 输出格式
输出一行一个整数表示答案对 $M$ 取模后的值。

```input1
4 5 3
```

```output1
2
```

## 提示
数列为 $\{0,4,4,3,2,0,2,2\},v_1=(4,3),v_2=(2,0),v_3=(2,2)$。

$v_1\cdot v_2 \bmod M=3,v_2\cdot v_3 \bmod M=4, v_1\cdot v_3 \bmod M=4$。

## 数据规模与约定
对于 $100\%$ 的数据，$1≤C≤10^9,1≤M≤10^9,1≤n≤3\times 10^5
(0\le i\le 2n)$。
## 题目来源
By yts1999


