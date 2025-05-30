## 题目描述

Up主家终于买电脑了，但是接下来有各种问题要处理。首要解决的问题就是网络问题。他要从移动公司开
始，通过一些基站来传递网络到他家。

为了简化问题，我们假设移动公司，所有的基站，Up主家位于同一条直线上，他们都位于这一条直线上的
某一点 $ x $，这些点不会重合。每个基站发射和接收的范围都是一个切于地面的圆，发射的半径 $ r_1 $ 是固定的，接收半径 $ r_2 $ 是可调的的。如下图：

![图一](./2556/file/pic1.jpg)

一个点 $ i $ 如果能从另一个点 $ j $ 接收到信号(当且仅当 $ x[j] < x[i] $ )，必须满足 $ i $ 的接收范围与 $ j $ 的发射范围相切，并且需要付 $ \sqrt{r_2[i]} $ 的额外费用。同时启动每一个点 $ i $ 都需要费用 $ v[i] $ .

当然一个点如果能够发射的Up主家只需要这个点的发射范围与Up主家所在的竖线相切或相交即可，如下

![图二](./2556/file/pic2.jpg)

当然费用越少就越好咯，于是Up主想要请你帮他的忙。

## 输入格式

第一行两个整数n,m.表示基站个数(包括移动公司)，up主家的坐标。(保证大等于所以基站的坐标)

接下来 $ n $ 行，每行三个整数 $ x[i],r_1[i],v[i] $ ,表示每个基站的坐标，发射范围以及费用。

$ x[i] $ 是按照坐标从小到大输入的，移动公司位于最小的那个坐标。

$ r_1 $ 为 $ 1,2……n $ 的排列。

## 输出格式

一个实数，保留小数点后三位。

## 样例输入

```
10 33
5 4 660
10 2 2040
11 6 3207
14 5 2006
18 3 6130
19 9 3363
22 1 1265
25 8 2836
27 10 7961
29 7 9075
```

## 样例输出

```
3501.000
```

## 数据规模与约定

对于 $100\%$ 的数据， $ n \leq 5 \times 10^6 $， $ x[i],m \leq 1\times 10^{12} $， $ v[i] \leq 1\times 10^4 $。