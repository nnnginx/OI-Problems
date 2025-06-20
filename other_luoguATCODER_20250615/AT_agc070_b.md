# AT_agc070_b [AGC070B] Odd Namori

## 题目描述

给定一个含有 $N$ 个顶点的有根树 $T$，顶点编号为 $1$ 到 $N$。其中，顶点 $1$ 为根节点，对于每一个顶点 $i$（$2 \leq i \leq N$），有 $p_i$ 为其父节点，且 $p_i < i$。

我们定义满足以下条件的有向图 $G$ 为“好图”：

- 每个顶点的出度都为 1。
- 图中不存在偶数长度的环。
- 对于所有 $2 \leq i \leq N$ 的 $i$，$G$ 中不包含边 $i \to p_i$。

计算所有可能的“好图”$G$ 中 $2^{\text{环的数量}}$ 的总和，再对 $998244353$ 取余。

## 输入格式

从标准输入读取：

> $N$ $p_2$ $p_3$ $\dots$ $p_N$

## 输出格式

输出所有“好图”中 $2^{\text{环的数量}}$ 的总和，再对 $998244353$ 取余后的结果。

## 输入输出样例 #1

### 输入 #1

```
2
1
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
3
1 2
```

### 输出 #2

```
34
```

## 输入输出样例 #3

### 输入 #3

```
5
1 2 1 1
```

### 输出 #3

```
3104
```

## 输入输出样例 #4

### 输入 #4

```
20
1 2 2 2 5 3 5 1 7 9 4 6 4 12 8 2 5 16 6
```

### 输出 #4

```
784973196
```

## 说明/提示

- $2 \leq N \leq 10^5$
- $1 \leq p_i < i$
- 所有输入的值均为整数

### 样例说明 1

两种可能的“好图”为：
1. 包含边 $1 \to 1$ 和 $2 \to 2$，环的数量为 2。
2. 包含边 $1 \to 2$ 和 $2 \to 2$，环的数量为 1。

所以，答案是 $(2^2 + 2^1) \bmod 998244353 = 6$。

### 样例说明 2

例如，边集包含 $1 \to 2$、$2 \to 3$ 和 $3 \to 1$ 的图是一个“好图”，其中有一个环。

### 样例说明 4

请注意，结果需要对 $998244353$ 取余。

 **本翻译由 AI 自动生成**