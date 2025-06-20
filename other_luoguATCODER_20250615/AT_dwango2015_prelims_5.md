# AT_dwango2015_prelims_5 電波局

## 题目描述

在某星球上，有一座呈正三角形布局的城镇，该城镇由 $N \times (N + 1) / 2$ 个房屋正三角形排列。这三角形的一边与东西方向平行，顶点是位于最北端的那所房子。

每栋房子由两个整数来编号。编号为 $(1, 1)$ 的是最北面的房子，第 $i$ 行(从北算起)中，第 $j$ 个(从西算起)房子的编号为 $(i, j)$，其中 $1 \leq j \leq i \leq N$。

以下是 $N = 5$ 的编号示例：

```
(1,1)
(2,1)(2,2)
(3,1)(3,2)(3,3)
(4,1)(4,2)(4,3)(4,4)
(5,1)(5,2)(5,3)(5,4)(5,5)
```

Dwango 公司目前拥有 $M$ 个广播站（编号为 $1$ 至 $M$），每个广播站都在一个以边与城镇外边界平行的正三角形范围内提供广播服务。

对于广播站 $i$（$1 \leq i \leq M$），其服务范围用三个整数 $a_i$、$b_i$、$c_i$ 表示。广播范围包括所有满足 $1 \leq k \leq j \leq c_i$ 的房子 $(a_i+j-1, b_i+k-1)$。

Dwango 公司计划新建一个广播站，为此已经设计了 $Q$ 种不同的方案。请编写程序，计算每种方案能带来多少新的客户。

## 输入格式

输入数据通过标准输入提供。格式如下：

> $N$ $M$ $a_1$ $b_1$ $c_1$ $a_2$ $b_2$ $c_2$ $\ldots$ $a_M$ $b_M$ $c_M$ $Q$ $d_1$ $e_1$ $f_1$ $d_2$ $e_2$ $f_2$ $\ldots$ $d_Q$ $e_Q$ $f_Q$

- 第一行包含两个整数 $N$（$1 \leq N \leq 1,000,000,000$）和 $M$（$1 \leq M \leq 1,000$）。
- 接下来的 $M$ 行，每行三个整数 $a_i$、$b_i$（$1 \leq b_i \leq a_i \leq N$）和 $c_i$（$1 \leq c_i \leq N - a_i + 1$），表示第 $i$ 个广播站服务的范围。此范围覆盖所有房子 $(a_i+j-1, b_i+k-1)$，对于所有满足 $1 \leq k \leq j \leq c_i$ 的整数 $j$ 和 $k$。
- 第 $M+2$ 行给出一个整数 $Q$（$1 \leq Q \leq 1,000$）。
- 接着的 $Q$ 行，每行包含三个整数 $d_i$、$e_i$（$1 \leq e_i \leq d_i \leq N$）和 $f_i$（$1 \leq f_i \leq N - d_i + 1$），表示构想中的新广播站服务范围。此范围覆盖所有房子 $(d_i+j-1, e_i+k-1)$，满足 $1 \leq k \leq j \leq f_i$ 的整数 $j$ 和 $k$。

## 输出格式

输出 $Q$ 行。第 $i$ 行为第 $i$ 种方案所能覆盖的新房子的数量。

## 输入输出样例 #1

### 输入 #1

```
8 3
2 2 4
5 4 3
6 1 3
2
4 1 4
7 6 2
```

### 输出 #1

```
5
2
```

## 输入输出样例 #2

### 输入 #2

```
3 2
1 1 2
3 2 1
3
2 1 2
2 2 1
1 1 3
```

### 输出 #2

```
1
0
2
```

## 说明/提示

### 部分分数

该题目有以下部分分数设置：

- 如果所有满足 $N \leq 200$ 且 $M \leq 200$ 以及 $Q \leq 200$ 的数据集都答对，可以得到 10 分。
- 如果所有满足 $M \leq 200$ 且 $Q \leq 200$ 的数据集都答对，可以在前者基础上再得 30 分。
- 对于没有额外限制的数据集，如果全答对，可以在前两者基础上再得 60 分，总计有 100 分。

### 样例解释

现有的三个广播站覆盖范围如图所示（○表示已覆盖，×表示未覆盖）：

```
× × ○ × ○ ○
× ○ ○ ○
× ○ ○ ○ ○
× × ○ ○
× ○ ○ ×
○ ○
× × × ×
```

对于第一种增设方案，新覆盖的房子在图中用 + 表示，共计 5 个：

```
× × ○ × ○ ○
+ ○ ○ ○
+ ○ ○ ○ ○
+ + ○ ○
× ○ ○ +
○ ○ ×
× × × ×
```

对于第二种增设方案，新覆盖的房子在图中用 + 表示，共计 2 个：

```
× × ○ × ○ ○
× ○ ○ ○
× ○ ○ ○ ○
× × ○ ○
× ○ ○ ×
○ ○
+ +
× ×
```

 **本翻译由 AI 自动生成**