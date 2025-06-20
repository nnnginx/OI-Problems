# AT_arc103_c [ARC103E] Tr/ee

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc103/tasks/arc103_c

给定一个长度为 $n$ 的字符串 $s$。是否存在满足以下条件的 $n$ 个顶点的树？

- 每个顶点被编号为 $1,2,\ldots,n$；
- 每条边被编号为 $1,2,\ldots,n-1$，其中第 $i$ 条边连接顶点 $u_i$ 和 $v_i$；
- 当 $s$ 的第 $i$ 个字符为 `1` 时，存在一种移除某条边的方式，使得能生成一个大小为 $i$ 的连通块；
- 当 $s$ 的第 $i$ 个字符为 `0` 时，无论如何移除一条边，都无法生成大小为 $i$ 的连通块；

如果存在满足条件的树，请构造一个符合条件的树。

## 输入格式

输入通过标准输入给出，格式如下：

> $ s $

## 输出格式

如果不存在满足条件的 $n$ 个顶点的树，输出 `-1`。

如果存在满足条件的 $n$ 个顶点的树，输出 $n-1$ 行。第 $i$ 行输出以空格分隔的 $u_i$ 和 $v_i$。若有多个符合条件的树，输出任意一个均可。

## 输入输出样例 #1

### 输入 #1

```
1111
```

### 输出 #1

```
-1
```

## 输入输出样例 #2

### 输入 #2

```
1110
```

### 输出 #2

```
1 2
2 3
3 4
```

## 输入输出样例 #3

### 输入 #3

```
1010
```

### 输出 #3

```
1 2
1 3
1 4
```

## 说明/提示

### 约束条件

- $2 \leq n \leq 10^5$
- $s$ 是由 `0` 和 `1` 组成的长度为 $n$ 的字符串

### 样例解释 1

从 $n$ 顶点的树中移除一条边无法生成大小为 $n$ 的连通块。

### 样例解释 2

移除第 1 条或第 3 条边会生成一个大小为 1 的连通块和一个大小为 3 的连通块。移除第 2 条边会生成两个大小为 2 的连通块。

### 样例解释 3

无论移除哪条边，都会生成一个大小为 1 的连通块和一个大小为 3 的连通块。

翻译由 DeepSeek R1 完成