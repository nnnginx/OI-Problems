## 题目描述

你可以把一个大小为 $n\times m$ 的大矩形分割成若干个矩形，要求分割出的矩形至少有一边在大矩形的边界上，比如下左图就是一种合法分割，下右图就是一种非法分割。

![](./3360/file/pic2.jpg)

一个大小为 $a\times b$ 的矩形的差异度是 $(ab-k)^2$，其中 $k$ 是给定常数。

你需要找到一种分割方案使得所有分割出的矩形的差异度之和最小，并输出这个最小值。

## 输入格式

一行三个整数 $n,m,k$。

## 输出格式

一行一个整数表示最小的差异度之和。

```input1
3 3 2
```

```output1
1
```

## 样例解释

按照题目描述中合法分割的例子为方案，得到的差异度之和为 $4\times (2-2)^2+1\times (1-2)^2=1$，可以证明这是最小的差异度之和。

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n,m\leq 300$，$0\leq k\leq 10^4$。

