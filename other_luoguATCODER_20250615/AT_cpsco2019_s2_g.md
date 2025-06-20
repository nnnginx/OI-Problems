# AT_cpsco2019_s2_g MSTX

## 题目描述

给定一个简单连通无向图，该图包含 $N$ 个顶点和 $M$ 条边。图中的第 $i$ 条边连接顶点 $u_i$ 和 $v_i$，其权重为 $w_i$。权重 $w_i$ 可以是一个正整数常数，也可以是一个变量 $x$。请解答以下 $Q$ 个查询。

- 对于每个查询，第 $i$ 个查询将提供一个正整数 $a_i$。
- 你的任务是计算当 $x = a_i$ 时，图的最小生成树的总权重。

## 输入格式

输入数据从标准输入中获取，具体格式如下：

字符 $c_i$ 为 `0` 或 `1`，用来标示 $w_i$ 是常数还是变量。如果 $c_i$ 为 `0`，则 $w_i$ 是一个正整数常数；如果 $c_i$ 为 `1`，则 $w_i$ 表示变量 $x$。

> $ N $ $ M $ $ u_1 $ $ v_1 $ $ c_1 $ $ w_1 $ $ u_2 $ $ v_2 $ $ c_2 $ $ w_2 $ $ \ldots $ $ u_M $ $ v_M $ $ c_M $ $ w_M $ $ Q $ $ a_1 $ $ a_2 $ $ \ldots $ $ a_Q $

## 输出格式

输出包含 $Q$ 行，分别对应每个查询的答案。第 $i$ 行应输出对于查询 $a_i$ 的结果。

## 输入输出样例 #1

### 输入 #1

```
3 3
1 2 0 1
2 3 0 5
3 1 1 x
3
4
5
6
```

### 输出 #1

```
5
6
6
```

## 输入输出样例 #2

### 输入 #2

```
9 15
1 3 0 954291757
2 3 1 x
2 4 1 x
1 5 0 138996221
2 5 0 353195922
3 5 1 x
4 5 0 913575467
1 6 0 824284691
1 7 1 x
2 7 1 x
1 8 0 131381221
6 8 0 208032501
7 8 0 973708325
5 9 1 x
6 9 0 298309896
5
215208399
554374432
47628333
810900084
87027328
```

### 输出 #2

```
1554451938
2793039057
625183720
3562616013
861577690
```

## 说明/提示

- 顶点数： $2 \le N \le 5 \times 10^4$
- 边数： $N - 1 \le M \le \min(5 \times 10^4, N(N-1)/2)$
- 对于每条边： $1 \le u_i, v_i \le N$ 且 $u_i \neq v_i$
- 边唯一性：任意两边 $i$ 和 $j$ 不可以满足 $(u_i, v_i) = (u_j, v_j)$ 或 $(u_i, v_i) = (v_j, u_j)$
- 图是连通的
- 常量边权重：当 $w_i$ 是常数时，满足 $1 \le w_i \le 10^9$
- 查询数： $1 \le Q \le 5 \times 10^4$
- 查询参数： $1 \le a_i \le 10^9$
- 输入中，除了 `x` 是字符，其他所有都是整数。

### 样例解释

在给定的例子中：
- 如果 $x \le 5$，那么最小生成树的权重为 $x + 1$。
- 如果 $x \ge 5$，那么最小生成树的权重为 $6$。

 **本翻译由 AI 自动生成**