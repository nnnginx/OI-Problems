## 题目背景
ICPC2020 WF G

## 题目描述
As with most types of products, buying a new phone can be difficult.
One of the main challenges is that there are a lot of different
aspects of the phone that you might care about, such as its price, its
performance, and how user-friendly the phone is.
Typically, there will be no single phone that is simultaneously the
best at all of these things: the cheapest phone, the most powerful
phone, and the most user-friendly phone will likely be different phones.

Thus when buying a phone, you are forced to make some sacrifices by
balancing the different aspects you care about against each other and
choosing the phone that achieves the best compromise (where "best"
of course depends on what your priorities happen to be).  One way of
measuring this sacrifice is known as the *opportunity cost*,
which (for the purposes of this problem) we define as follows.

Suppose that you have bought a phone with price $x$, performance $y$,
and user-friendliness $z$. For simplicity, we assume that these three
values are measured on a comparable numeric scale where higher is
better. If there are $n$ available phones, and the values
$(x_i,y_i,z_i)$ represent the (price, performance, user-friendliness)
of the $i^{\text{th}}$ phone, then the opportunity cost of your phone
is defined as

$$\max _{1 \leq i \leq n}\left(\max \left(x_{i}-x, 0\right)+\max \left(y_{i}-y, 0\right)+\max \left(z_{i}-z, 0\right)\right)$$


Write a program that, given the list of available phones, finds a
phone with the minimum opportunity cost.

## 输入格式
The first line of input contains an integer $n$ ($2 \leq n \leq
200\,000$), the number of phones considered. Following that are $n$ lines.
The $i^{\text{th}}$ of these lines contains three integers $x_i$, $y_i$, and $z_i$,
where $x_i$ is the price, $y_i$ is the performance, and $z_i$ is the
user-friendliness of the $i^{\text{th}}$ phone ($1 \leq x_i, y_i, z_i \leq
10^9$).

## 输出格式
Output a single line containing two integers: the smallest possible
opportunity cost and an integer between $1$ and $n$ indicating the
phone achieving that opportunity cost. If there are multiple such
phones, output the one with the smallest index.


## 题目大意
与大多数类型的产品一样，购买一部新手机可能很困难。其中一个主要困难是，你可能会关心手机的许多不同方面，比如价格、性能以及手机的用户友好程度（**本题中仅考虑这三种因素**）。通常情况下，不会有一款手机同时在所有这些方面都是最好的，也就是说，最便宜的手机、功能最强大的手机和用户最友好的手机可能是不同的手机。因此，在购买手机时，你不得不做出一些牺牲，平衡彼此关心的不同方面，并选择实现最佳折衷的手机（当然，“最佳”取决于你的优先级）。衡量这种牺牲的一种方法称为**机会成本**（为了解决这个问题），我们将其定义如下：

某商店里一共有 $n$ 部手机，其中第 $i$ 部手机的价格为 $x_i$，性能为 $y_i$，用户友好程度为 $z_i$。假设你购买了一个价格为 $x$，性能为 $y$，用户友好程度为 $z$ 的一台手机，那么购买这台手机的机会成本用如下公式表示：

$$\max\limits_{1\leqslant i\leqslant n}(\max(x_i-x,0)+\max(y_i-y,0)+\max(z_i-z,0))$$

现在，请求出所有 $n$ 部手机的机会成本的最小值，并找到机会成本最小的**编号最小**的手机的编号。

数据范围：

- $2\leqslant n\leqslant 2\times 10^5$。
- $1\leqslant x_i,y_i,z_i\leqslant 10^9$。

Translated by Eason_AC

```input1
4
20 5 5
5 20 5
5 5 20
10 10 10
```

```output1
10 4

```

```input2
4
15 15 5
5 15 15
15 5 15
10 10 10
```

```output2
10 1
```

