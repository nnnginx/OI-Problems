# AT_agc001_c [AGC001C] Shorten Diameter

## 题目描述

给你一棵 $N$ 个点的无向树，定义点 $u$ 和 $v$ 之间的距离是从 $u$ 到 $v$ 的简单路径上的边数。

你需要删除一些点，使树的直径小于等于 $K$，当且仅当删除某点不会对树的联通性产生影响时才可以删除。问至少删除多少点才可以满足要求。

## 输入格式

>
>第一行两个个整数 $N, K$。
>
>之后 $N - 1$ 行描述一棵树。
>

## 输出格式

>
>一个整数，表示最少删掉点的个数。

感谢 @ToBiChi 提供翻译

## 输入输出样例 #1

### 输入 #1

```
6 2
1 2
3 2
4 2
1 6
5 6
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
6 5
1 2
3 2
4 2
1 6
5 6
```

### 输出 #2

```
0
```

## 说明/提示

$2≤N≤2000$，$1≤K≤N-1$，保证给出的图是一棵树。