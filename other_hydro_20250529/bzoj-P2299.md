## 题目描述

给你一对数 $a,b$，你可以任意使用 $(\pm a,\pm b)$ 这些向量，问你能不能拼出另一个向量 $(x,y)$。

说明：这里的拼就是使得你选出的向量之和为 $(x,y)$。

## 输入格式

第一行一个整数 $T$ 表示数据组数。

接下来 $T$ 行每行四个整数 $a,b,x,y$ 表示一组数据。

## 输出格式

共 $T$ 行，每行一个字符 `Y` 表示能拼出或 `N` 表示不能拼出。

```input1
3
2 1 3 3
1 1 0 1
1 0 -2 3
```

```output1
Y
N
Y
```

## 样例解释

第一组：$(2,1)+(1,2)=(3,3)$；

第三组：$(-1,0)+(-1,0)+(0,1)+(0,1)+(0,1)=(-2,3)$。

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq T\leq 5\times 10^4$，$|a|,|b|,|x|,|y|\leq 2\times 10^9$。

