## 题目描述
给出一个环，上面有 $n$ 个点，每个相邻的点对之间的距离为 $1$。

每个点有两个属性 $a_i$ 和 $b_i$，对于点 $i$，定义 $f_i$ 为它与满足 $i\ne j$ 且 $a_j\ge b_i$ 的 $j$ 与 $i$ 在环上的最短距离。特殊地，如果没有满足条件的 $j$，其 $f_i=-1$。

## 输入格式
输入共 $3$ 行。\
第 $1$ 行 $1$ 个整数 $n$ 。\
第 $2$ 行 $n$ 个整数，其中第 $i$ 个表示 $a_i$，意义同上。\
第 $3$ 行 $n$ 个整数，其中第 $i$ 个表示 $b_i$，意义同上。

## 输出格式
输出 $1$ 行 $n$ 个整数，其中第 $i$ 个表示 $f_i$，意义同上。

```input1
3
1 2 3
3 2 1
```

```output1
1 1 1
```

```input2
5
5 4 3 5 6
7 6 5 4 3
```

```output2
-1 2 1 1 1
```

```input3
5
1 1 2 1 1
2 2 2 2 2
```

```output3
2 1 -1 1 2
```

## 提示
### 数据规模与约定

对于 $20\%$ 的数据，$1\le n \le 10^3$；\
对于 $100\%$ 的数据，$1\le n \le 10^5$，$1\le a_i,b_i\le 10^9$。

我们对于测试点 $4$ 至 $11$ 采用捆绑测试。

### 样例 1 解释
对于 $i=1$，$a_3=3= b_1=3$, $1$ 和 $3$ 的距离是 $1$，所以 $f_1=1$。\
对于 $i=2$，$a_3=3> b_2=2$, $2$ 和 $3$ 的距离是 $1$，所以 $f_2=1$。\
对于 $i=3$，$a_2=2> b_3=1$, $2$ 和 $3$ 的距离是 $1$，所以 $f_3=1$。

$\text{Upd 2021.3.30}$：增加一组 hack 数据。


