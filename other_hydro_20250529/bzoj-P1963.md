## 题目描述

$F$ 是一个整数 $\to$ 整数的函数，换句话说，$F$ 在所有整数上有定义，对于任何一个整数 $x$，$F(x)$ 是一个整数。现在给一个整数 $c$。如果对于所有的整数 $x$，下面这个等式都满足，那么 $F$ 就被叫做 $c-\text{beautiful}$ 函数。

$$
F(2 \cdot F(x)-x+1)=F(x)+c
$$

输出下面这个式子当 $F$ 是一个 $c-\text{beautiful}$ 函数的时候可能的最小值。

$$
\sum^{n-1}_{i=0}\left|F(x_i)-y_i\right|
$$

使用下列方法生成 $x_i$ 和 $y_i$。

```cpp
x[0] = xzero
x[i] = (x[i - 1] * xprod + xadd) % xmod
y[0] = yzero
y[i] = (y[i - 1] * yprod - yadd) % ymod
```

## 输入格式

输入共一行，$10$ 个正整数，依次为 $c,n,xzero,xprod,xadd,xmod,yzero,yprod,yadd,ymod$。

## 输出格式

输出共一行，为所求的最小值。

```input1
4 10 0 1 1 456 1 1 1 456
```
```output1
5
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le c \le 16$，$1 \le n \le 10^4$，$1 \le xmod,ymod \le 10^9$，$0 \le xzero,xprod,xadd$。

