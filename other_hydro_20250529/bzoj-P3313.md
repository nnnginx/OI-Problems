## 题目描述

FJ 喜欢收集不同的奶牛，他将未有的 $N$ 头奶牛用如下的形式描述：

Farmer John has no large brown noisy cow.

Farmer John has no small white silent cow.

Farmer John has no large spotted noisy cow.

每一行，描述一头 FJ 未有的牛。

每一行都含有相同个数的形容词。

在以上给出的列表中，每行共有 $3$ 个形容词，第一个形容词有两种（large 和 small），第二个形容词有 $3$ 种（brown, white 和 spotted），第三个形容词有 $2$ 种（noisy 和 silent）。

所以共可以组成 $12$ 头不同的奶牛，除了列表给出的 $3$ 头，他已经拥有了其他 $9$ 头。

若将FJ已经拥有的牛按形容词的字典序排序，请问他已有的第 $K$ 头牛是哪一头。

## 输入格式

第一行两个整数 $N,K$。

接下来 $N$ 行，每行一个字符串，描述了一头 FJ 没有的牛。

## 输出格式

一行，表示答案。

```input1
3 7
Farmer John has no large brown noisy cow.
Farmer John has no small white silent cow.
Farmer John has no large spotted noisy cow.
```

```output1
small spotted noisy
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq N\leq 100$，形容词数量在 $2\sim 30$ 的范围内，牛的数量至多为 $10^9$。

## 题目来源

Silver

鸣谢 Alegria\_ 提供译文