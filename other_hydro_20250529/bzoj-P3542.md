## 题目描述

在一片 $m \times m$ 的地上．驻扎着 $n$ 个军队,编号依次为 $1 \sim n$,第 $i$ 个军队的位置可用二元组 $(x_i,y_i)$ 表示，可能有多个军队驻扎在同一个位置。

接下来有 $t$ 个时刻，每个时刻会发生下列两种事件之一：

1. 第 $x$ 个军队向一个方向（向上（`U`）向下（`D`）向左（`L`）向右（`R`））移动了 $d$ 个单位。
2. 第 $x$ 个军队需要集结和它在同一行或同一列的且编号在 $[l,r]$ 的军队，也就是说，这些军队需要赶到第 $x$ 个军队的驻地。

定义第 $i$ 个军队赶到第 $j$ 个军队所需的花费为 $cost(i,j)=(x_i-x_j)^2+(y_i-y_j)^2$。

请你输出每次集结时，所有被集结的军队的花费之和，对 $10^9+7$ 取模。

## 输入格式

第一行，两个数 $n$ 和 $m$。

接下来 $n$ 行，每行两个数 $x_i,y_i$。

接下一行，一个数 $t$。

接下来 $t$ 行，每行的格式为下列两种格式之一：

1. `S x d`，其中 $S \in \{U,L,D,R\}$，代表第一种事件。
2. `Q x L R`，代表第二种事件。

为了体现在线询问,每次你读进 $x'$ 后，真正的 $x = x' \oplus lastans$，其中 $lastans$ 是上一次答案对 $10^9+7$ 取模后的结果，一开始 $lastans=0$。

## 输出格式

对于每一个 `Q` 事件，输出一个答案，对 $10^9+7$ 取模。

```input1
5 3
1 2
2 2
3 2
2 1
2 3
7
Q 2 1 5
Q 6 3 4
D 1 1
Q 0 1 5
Q 7 1 5
L 5 1
Q 4 1 5
```
```output1
4
2
3
6
4
```

解密后的输入：

```plain
Q 2 1 5
Q 2 3 4
D 3 1
Q 2 1 5
Q 4 1 5
L 3 1
Q 2 1 5
```

![](./3092/file/pic1.jpg)

## 提示

$n \le 10^5,~m \le 10^{18}$。保证军队在移动过程中不会超出边界。每个军队集结后会回到原来的驻地。

## 题目来源

By Dzy
