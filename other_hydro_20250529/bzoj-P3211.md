## 题目描述

花神喜欢步行游历各国，顺便虐爆各地竞赛花神有一条游览路线，它是线型的，也就是说，所有游历国家呈一条线的形状排列，花神对每个国家都有一个喜欢程度（当然花神并不一定喜欢所有国家）每一次旅行中，花神会选择一条旅行路线，它在那一串国家中是连续的一段，这次旅行带来的开心值是这些国家的喜欢度的总和，当然花神对这些国家的喜欢程度并不是恒定的，有时会突然对某些国家产生反感，使他对这些国家的喜欢度 $x$ 变为 $\left\lfloor\sqrt x\right\rfloor$，也就是开根号（可能是花神虐爆了那些国家的 OI，从而感到乏味）现在给出花神每次的旅行路线，以及开心度的变化，请求出花神每次旅行的开心值。

## 输入格式

第一行是一个整数 $n$ 表示有 $n$ 个国家。

第二行有 $n$ 个空格隔开的整数，表示每个国家的初始喜欢度 $a_i$。

第三行是一个整数 $m$ 表示有 $m$ 条信息要处理。

第四行到最后，每行三个整数 $x,l,r$（$l\leq r$）。

- 当 $x=1$ 时询问国家 $l$ 到 $r$ 的开心值总和；
- 当 $x=2$ 是国家 $l$ 到 $r$ 中每个国家的喜欢度 $\left\lfloor\sqrt x\right\rfloor$。

提示：对于 C++ 选手，建议使用 `sqrt` 函数，且向下取整。

## 输出格式

每次 $x=1$ 时，每行一个整数，表示这次旅行的开心度。

```input1
4
1 100 5 5
5
1 1 2
2 1 2
1 1 2
2 2 3
1 1 4
```

```output1
101
11
11
```

## 数据范围

对于 $100\%$ 的数据， $n\le 10^5$，$m\le 2 \times 10^5$，$0 \leq a_i \leq 10^9$。

## 来源

SPOJ 2713 GSS4