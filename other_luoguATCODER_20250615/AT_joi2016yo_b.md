# AT_joi2016yo_b ゼッケンの交換 (Swapping Bibs)

## 题目描述

### 题目简述

给定一个由 $n$ 个正整数组成的数列 $a=(a_1,a_2,...,a_n)$ ，并给定一个整数 $m$ 。请按照 $k=1,2,...,m$ 的顺序执行以下操作：

令 $i=1$ 。当 $i<n$ 时，如果 $a_i$ $\bmod$ $k>a_{i+1}$  $\bmod$ $k$ ，则交换 $a_i$ 和 $a_{i+1}$ 的值；否则什么都不做。然后，将 $i$ 加 $1$ 。当 $i=n$ 时，将 $i$ 的值恢复为 $1$ ，本轮操作结束。

现在，输入给出 $n,m$ 以及 $a$ 开始时的数据，请在所有操作完成后输出 $a$ 数列所有元素的值。

## 输入格式

输入 $(n+1)$ 行。第一行是两个正整数 $n,m$ ，中间以单个空格隔开。接下来的 $n$ 行中，每行输入一个整数，全部输入中的第 $(i+1)$ 行输入的整数为 $a_i$ 。

## 输出格式

输出 $n$ 行，每行一个正整数，其中第 $i$ 行的数字为在所有操作完成后的 $a_i$ 的值。

## 输入输出样例 #1

### 输入 #1

```
6 4
3
2
8
3
1
5
```

### 输出 #1

```
2
3
1
8
5
3
```

## 输入输出样例 #2

### 输入 #2

```
10 6
1
2
3
4
5
6
7
8
9
10
```

### 输出 #2

```
6
1
2
3
10
4
8
7
9
5
```