# AT_arc036_b [ARC036B] 山のデータ

## 题目描述

现在，有 $N$ 个地点。从西起第 $i(1 \le i \le N)$ 个地点的高度为 $h_i$。

这样，就有了一个三元组 $(s，t，u)$，$(1 \le s \le t \le u \le N)$。

那么，这一个三元组是山，当且仅当：

对于满足 $s \le i \le t-1$ 的任意整数中的 $i$，满足 $h_i < h_{i+1}$ 且在对于满足 $t \le i \le u-1$ 的任意整数中的 $i$，满足 $h_i > h_{i+1}$。

现在，需要找出山的**最大**长度。（定义山的长度为 $u - s + 1$）。

## 输入格式

第一行，一个整数 $N$。

第二行到第 $N + 1$ 行，每行一个整数 $h_i$。表示第 $i$ 个地点的高度。

## 输出格式

一个整数，表示山的**最大**长度。（定义山的长度为 $u - s + 1$）。

## 输入输出样例 #1

### 输入 #1

```
6
4
5
1
6
9
7
```

### 输出 #1

```
4
```

## 输入输出样例 #2

### 输入 #2

```
7
90
70
50
30
20
10
5
```

### 输出 #2

```
7
```

## 说明/提示

$1 \le N \le 3 \times 10^5, 1 \le h_i \le 10^9$。

每一个 $h_i$ 互不相同（即对于 $1 \le i < j \le N$，$h_i \ne h_j$）。