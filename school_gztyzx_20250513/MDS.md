# MultiDimensional

## 题目描述

你最近研究了一些物理内容，对于『维度』特别感兴趣。

你现在在一个 $n$ 维的世界里，你初始时在原点上，你要移动到一个点 $Des(g,g,.....,g)$ 上。

你现在没有太强的能力。

你一步只能走向一个相邻的点。

你要从 $Des$ 往原点走。

特别地，你是入门者，所以 $g=\neg\left[\left(\neg p \land q\right) \vee \left(q \oplus p \rightarrow q \right)\right] \leftrightarrow \left[\left(p \land \neg q \right)\land \left(q \oplus p \vee q\right) \vee p \right] \land \neg q$ ， $q^p = 1$

你很聪明，所以请问：你最多能找到多少条从 $Des$ 到 原点的路径，使得所有的路径都不与别的路径在过程中有交点？

你太聪明了，所以你要构造一组满足所有条件的路径。

但是你要反过来输出路径。

## 输入格式

一行，一个整数 $n$ 。

## 输出格式

输出共 $ans+1$ 行。

第一行，一个整数 $ans$ 。

接下来 $ans$ 行，每行输出一条合法路径。

**不要输出多余的行末空格，否则SPJ会判错** 。

## 样例1

### 输入样例1

```
1
```

### 输出样例1

```
1
0 1
```

## 提示

由于本题的特殊性质，本题采用SPJ。

路径的表示方法:

原点 $A$ $B$ ... $Des$

其中 $A$ , $B$ ... 是一个压缩二进制得到的数，表示一个 坐标。

我们把每个坐标看作一个 $g+1$ 进制数，把他们从第一项开始连成一个数，然后转换为10进制即可。

比如若 $g=7$ 时，坐标 $C(3,4,1)$ 应转换为 $8$ 进制数 $341$ ，然后转换为十进制数 $225$ 输出。

比如，当 $n=2$ 时，若 $g=3$ ，则路径： $K_1(1,1) \rightarrow K_2(1,2) \rightarrow K_3(2,2)$ 应该输出为 $5$ $6$ $10$

对于 $100\%$ 的数据， $3 \le n \le 62$ 。

