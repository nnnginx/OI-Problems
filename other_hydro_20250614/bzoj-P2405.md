## 题目描述

小 D 喜欢的数有这样的性质： 令 $n$为正整数，$\operatorname{S}(n)$为 $n$ 的各位数字之和，令

$$
\operatorname{D}(n) = \left\{

\begin{aligned}

& \operatorname{S}(n) ,            & \operatorname{S}(n) < 10\\
& \operatorname{D}(\operatorname{S}(n)) ,        &\operatorname{S}(n)\ge 10\\

\end{aligned}

\right.
$$

小 D 喜欢的数一定能表示成 $x \times \operatorname{D}(x) $ 这种形式。（即若一个数 $A$ 是被喜欢的，则存在一个正整数 $x$ ，使得 $A = x \times \operatorname{D}(x)$ ）

小 D 想知道在区间 $[L , R]$ 中，有多少个数是他喜欢的。

## 输入格式

第一行一个整数 $T$ ，表示数据组数。

以下每一行两个整数 $L,R$ ，代表询问 $[L, R]$ 。

## 输出格式

输出 $T$ 行，每行一个整数，表示在这个区间内小 D 喜欢的数出现了多少次。

```input1
3
1 5
3 9
8 8
```

```output1
2
2
0
```

## 数据规模与约定

对于 $100\%$  的数据，保证 $1\le L\le R \le 10^{18} , T\le 20$ 。
