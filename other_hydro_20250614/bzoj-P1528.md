## 题目描述

Jasio 是一个三岁的小男孩，他最喜欢玩玩具了，他有 $n$ 个不同的玩具，它们都被放在了很高的架子上所以 Jasio 拿不到它们。为了让他的房间有足够的空间，在任何时刻地板上都不会有超过 $k$ 个玩具。Jasio 在地板上玩玩具。Jasio 的妈妈则在房间里陪他的儿子。当 Jasio 想玩地板上的其他玩具时，他会自己去拿，如果他想玩的玩具在架子上，他的妈妈则会帮他去拿，当她拿玩具的时候，顺便也会将一个地板上的玩具放上架子使得地板上有足够的空间。他的妈妈很清楚自己的孩子所以他能够预料到 Jasio 想玩些什么玩具。所以她想尽量的使自己去架子上拿玩具的次数尽量的少，应该怎么安排放玩具的顺序呢?

## 输入格式

In the first line of the standard input there are three integers: $n$,$k$,$p$, separated by single spaces. These denote respectively: the total number of cars, the number of cars that can remain on the floor at once and the length of the sequence of cars which Johnny will want to play with. Each of the following $p$ lines contains one integer. These integers are the numbers of cars Johnny will want to play with (the cars are numbered from $1$ to $n$).

## 输出格式

In the first and only line of the standard output one integer should be written - the minimal number of times his mother has to pick a car from the shelf.

```input1
3 2 7
1
2
3
1
3
1
2
```
```output1
4
```

## 数据规模及约定

对于 $100 \%$ 的数据 ： $1\le k\le n\le 100\ 000$, $1\le p\le 5 \times 10^5$。
