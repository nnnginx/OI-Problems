## 题目描述

求多项式 $(x^2+x+1)^n$ 展开后第 $i$ 项的系数。

## 输入格式

第一行一个整数 $T$ 表示数据组数。

接下来 $T$ 行，每行两个整数 $n,i$ 表示一组询问。

## 输出格式

对于每组询问，输出一行一个整数表示对应询问在 $\text{mod }3$ 意义下的答案。

```input1
5
2 0
7 4
4 5
5 3
8 15
```

```output1
1
2
1
0
2
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq T\leq 10^4$，$0\leq n\leq 10^{15}$，$0\leq i\leq 2\times n$。

