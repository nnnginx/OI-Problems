## 题目描述

小 L 今天学习了 Kleene 三值逻辑。

在三值逻辑中，一个变量的值可能为：真（`True`，简写作 `T`）、假（`False`，简写作 `F`）或未确定（`Unknown`，简写作 `U`）。

在三值逻辑上也可以定义逻辑运算。由于小 L 学习进度很慢，只掌握了逻辑非运算 $\lnot$，其运算法则为：

$$
\lnot \texttt{T} = \texttt{F}, \lnot \texttt{F} = \texttt{T}, \lnot\texttt{U} = \texttt{U}.
$$

现在小 L 有 $n$ 个三值逻辑变量 $x_1,\cdots, x_n$。小 L 想进行一些有趣的尝试，于是他写下了 $m$ 条语句。语句有以下三种类型，其中 $\gets$ 表示赋值：

1. $x_i \gets v$，其中 $v$ 为 `T`，`F`，`U` 的一种；
2. $x_i \gets x_j$；
3. $x_i \gets \lnot x_j$。

一开始，小 L 会给这些变量赋初值，然后按顺序运行这 $m$ 条语句。

小 L 希望执行了所有语句后，所有变量的最终值与初值都相等。在此前提下，小 L 希望初值中 `Unknown` 的变量尽可能少。

在本题中，你需要帮助小 L 找到 `Unknown` 变量个数最少的赋初值方案，使得执行了所有语句后所有变量的最终值和初始值相等。小 L 保证，至少对于本题的所有测试用例，这样的赋初值方案都必然是存在的。

## 输入格式

**本题的测试点包含有多组测试数据。**

输入的第一行包含两个整数 $c$ 和 $t$，分别表示测试点编号和测试数据组数。对于样例，$c$ 表示该样例与测试点 $c$ 拥有相同的限制条件。

接下来，对于每组测试数据：

- 输入的第一行包含两个整数 $n$ 和 $m$，分别表示变量个数和语句条数。
- 接下来 $m$ 行，按运行顺序给出每条语句。
  
  - 输入的第一个字符 $v$ 描述这条语句的类型。保证 $v$ 为 `TFU+-` 的其中一种。
  - 若 $v$ 为 `TFU` 的某一种时，接下来给出一个整数 $i$，表示该语句为 $x_i \gets v$；
  - 若 $v$ 为 `+`，接下来给出两个整数 $i,j$，表示该语句为 $x_i \gets x_j$；
  - 若 $v$ 为 `-`，接下来给出两个整数 $i,j$，表示该语句为 $x_i \gets \lnot x_j$。

## 输出格式

对于每组测试数据输出一行一个整数，表示所有符合条件的赋初值方案中，`Unknown` 变量个数的最小值。

```input1
1 3
3 3
- 2 1
- 3 2
+ 1 3
3 3
- 2 1
- 3 2
- 1 3
2 2
T 2
U 2
```

```output1
0
3
1
```

## 样例 1 解释

第一组测试数据中，$m$ 行语句依次为

- $x_2 \gets \lnot x_1$；
- $x_3 \gets \lnot x_2$；
- $x_1 \gets x_3$。

一组合法的赋初值方案为 $x_1 = \texttt{T}, x_2 = \texttt{F}, x_3 = \texttt{T}$，共有 $0$ 个`Unknown` 变量。因为不存在赋初值方案中有小于 $0$ 个`Unknown` 变量，故输出为 $0$。

第二组测试数据中，$m$ 行语句依次为

- $x_2 \gets \lnot x_1$；
- $x_3 \gets \lnot x_2$；
- $x_1 \gets \lnot x_3$。

唯一的赋初值方案为 $x_1 = x_2 = x_3 = \texttt{U}$，共有 $3$ 个`Unknown` 变量，故输出为 $3$。

第三组测试数据中，$m$ 行语句依次为

- $x_2 \gets \texttt{T}$；
- $x_2 \gets \texttt{U}$。

一个最小化 `Unknown` 变量个数的赋初值方案为 $x_1 = \texttt{T}, x_2 = \texttt{U}$。$x_1 = x_2 = \texttt{U}$ 也是一个合法的方案，但它没有最小化 `Unknown` 变量的个数。

## 样例 2

见附加文件的 [`tribool2.in`](./417/file/tribool2.in) 和 [`tribool2.ans`](./417/file/tribool2.ans)。

该组样例满足测试点 $2$ 的条件。

## 样例 3

见附加文件的 [`tribool3.in`](./417/file/tribool3.in) 和 [`tribool3.ans`](./417/file/tribool3.ans)。

该组样例满足测试点 $5$ 的条件。

## 样例 4

见附加文件的 [`tribool4.in`](./417/file/tribool4.in) 和 [`tribool4.ans`](./417/file/tribool4.ans)。

该组样例满足测试点 $8$ 的条件。

## 数据范围

对于所有测试数据，保证：

- $1 \le t \le 6$，$1 \le n,m \le 10 ^ 5$；
- 对于每个操作，$v$ 为 `TFU+-` 中的某个字符，$1 \le i,j \le n$。

| 测试点编号 | $n,m\leq$ | $v$ 可能的取值 |
| :-: | :-: | :-: |
| $1\sim 2$ | $10$ | `TFU` |
| $3$ | $10^3$ | `TFU` |
| $4$ | $10^5$ | `TFU` |
| $5$ | $10^3$ | `U+` |
| $6$ | $10^5$ | `U+` |
| $7$ | $10^3$ | `+-` |
| $8$ | $10^5$ | `+-` |
| $9$ | $10^3$ | `TFU+-` |
| $10$ | $10^5$ | `TFU+-` |