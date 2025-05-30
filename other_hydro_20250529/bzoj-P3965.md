## 题目描述

如果你有足够的石块，那么建一座金字塔绝不算难事。举个例子，在一块平地上，我们铺一个 $10\times 10$ 的矩形，然后在 $10\times 10$ 的矩形上面铺一个 $9\times 9$ 的，然后 $8\times 8$ 的……以此类推，直到顶上 $1\times 1$。这个金字塔有 $10$ 层，我们称这类金字塔为“高金字塔”。

如果你认为这样的金字塔太陡了，那么我们有办法让他看上去坡度平缓一些。比如，在 $10\times 10$ 的矩形上，我们铺一个 $8\times 8$ 的矩形，然后是 $6\times 6$ 的……这样的金字塔只有 $5$ 层了，大约为底座边长的一半。我们称之为“矮金字塔”。

很久以前，一位法老从父亲那儿继承了一大堆用于搭建金字塔的石块。他决定用这些石块搭建一座金字塔——每个石块都必须用上。建筑师告诉他，这样的要求不一定能实现。例如，如果你有 $10$ 块石头，那么可以搭一个底座为$3$ 的矮金字塔；如果有 $5$ 块石头，那么就搭一个底座为 $2$ 的高金字塔。如果你有 $7$ 块石头呢？不幸的是，确实找不出一种搭金字塔的方案了。

思考再三后，法老决定放低要求——搭不止一座金字塔。但是仍然要满足如下几个条件：

- 所有石块都必须用上；

- 金字塔数要尽可能少；

- 所有金字塔两两不同；

- -金字塔至少包含两层，即底座为 $1$ 的金字塔和底座为 $2$ 的矮金字塔是不允许的；

- 满足以上 $4$ 点的基础上，最大的金字塔要尽可能大（大定义为用的石块数多）；

- 满足以上 $5$ 点的基础上，次大的金字塔要尽可能大；

- 以此类推……

你能求出最好的搭金字塔方案么？或者告诉法老这是做不到的。

## 输入格式

输入仅包含一行一个正整数 $n$，表示你拥有的石块数量。

## 输出格式

输出需要给出具体的方案，或者告诉法老不可能办到。

具体的，如果不能办到，输出 `impossible`；否则输出每个金字塔如何搭建，格式是 `底座长度+H/L`，`H` 表示这是一座高金字塔，`L` 表示矮金字塔。

多座金字塔按从大到小排序输出，如果大小一样，先输出“高金字塔”。

两座金字塔间用恰好一个空格隔开。

```input1
29
28
0
```

```output1
Case 1: 3H 3L 2H
Case 2: impossible
```

## 数据规模与约定

对于 $100\%$ 的数据，$0\leq n\leq 10^6$。

