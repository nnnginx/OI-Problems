## 题目描述

对于方程 $\sum_{i=1}^nw_it_i=S$ 这个方程，设其有不少于 $p$ 组解。

现在给出 $n,p,w_{1\cdots n}$，请输出最小的 $S$。

注意 $t_{1\cdots n}$ 均为非负整数。

## 输入格式

第一行给出数字 $n$。

第二行 $n$ 个数，代表 $w_{1\cdots n}$。

第三行一个数字 $m$，代表有 $m$ 个询问。

第四行 $m$ 个数，每个数字代表一个 $p$。

## 输出格式

$m$ 行，每行一个数 $S$，对应于相应的 $p$。

```input1
3
1 1 2
3
2 3 6
```

```output1
1
2
3
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq 5$，$1\leq w_i,m\leq 10$，$1\leq p,S\leq 10^{18}$。

