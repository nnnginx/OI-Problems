# AT_code_thanks_festival_2017_h Union Sets

## 题目描述

开始时，有 $N$ 个互不相交的集合，分别为 $\{1\}, \{2\}, \ldots, \{N\}$。接下来会进行 $M$ 次合并操作。在第 $i (1 \le i \le M)$ 次操作中，你需要合并包含元素 $a_i$ 和 $b_i$ 的两个集合。如果这两个元素已经在同一个集合中，则不进行任何合并。

随后，会有 $Q$ 个查询。对于每个查询 $j (1 \le j \le Q)$，你需要回答：

- 元素 $x_j$ 和 $y_j$ 第几次操作之后被合并在同一个集合中？

如果在 $M$ 次操作结束后，$x_j$ 和 $y_j$ 仍然不在同一个集合中，输出 `-1`。如果它们在某次操作后合并到同一个集合，请输出使得它们第一次处于同集合的最小操作序号 $K (1 \le K \le M)$。

## 输入格式

输入使用以下格式：

> $N$ $M$ $a_1$ $b_1$ $\ldots$ $a_M$ $b_M$ $Q$ $x_1$ $y_1$ $\ldots$ $x_Q$ $y_Q$

## 输出格式

对于每个查询，输出其答案。第 $j (1 \le j \le Q)$ 行应是第 $j$ 个查询的结果。

## 输入输出样例 #1

### 输入 #1

```
7 5
1 2
3 4
2 1
2 3
4 1
5
1 2
3 4
1 4
2 3
6 7
```

### 输出 #1

```
1
2
4
4
-1
```

## 输入输出样例 #2

### 输入 #2

```
7 6
1 2
1 3
1 4
1 5
1 6
1 7
3
1 3
4 5
6 7
```

### 输出 #2

```
2
4
6
```

## 输入输出样例 #3

### 输入 #3

```
10 0
5
1 2
4 3
5 6
8 7
9 10
```

### 输出 #3

```
-1
-1
-1
-1
-1
```

## 说明/提示

- $2 \le N \le 10^5$
- $0 \le M \le 10^5$
- $1 \le a_i, b_i \le N$
- $a_i \ne b_i$
- $1 \le Q \le 10^5$
- $1 \le x_j, y_j \le N$
- $x_j \ne y_j$
- 所有输入均为整数。

### 示例说明

初始时，有 $7$ 个集合 $\{1\}, \{2\}, \{3\}, \{4\}, \{5\}, \{6\}, \{7\}$。接下来的 $5$ 次合并操作使得集合状态依次为：
- 第 1 次操作后：$\{1, 2\}, \{3\}, \{4\}, \{5\}, \{6\}, \{7\}$
- 第 2 次操作后：$\{1, 2\}, \{3, 4\}, \{5\}, \{6\}, \{7\}$
- 第 3 次操作后：$\{1, 2\}, \{3, 4\}, \{5\}, \{6\}, \{7\}$
- 第 4 次操作后：$\{1, 2, 3, 4\}, \{5\}, \{6\}, \{7\}$
- 第 5 次操作后：$\{1, 2, 3, 4\}, \{5\}, \{6\}, \{7\}$

 **本翻译由 AI 自动生成**