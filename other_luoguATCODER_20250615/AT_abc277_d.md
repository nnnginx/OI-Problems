# AT_abc277_d [ABC277D] Takahashi's Solitaire

## 题目描述

【题面翻译】

给定 $n$ 张牌，每张牌上有一个数字 $a_i$。

你要先选一张牌放在桌子上。假设当前最后一张放置的牌为 $x$，接下来，你每次只能放写着 $x$ 或 $(x + 1) \bmod m$ 的牌。

一直操作下去。你需要让你手上剩下的牌的总和**最小**。

translated by @[liangbowen](https://www.luogu.com.cn/user/367488).

## 输入格式

第一行两个数 $n$，$m$。

接下来 $n$ 个数，表示卡牌上的数字 $a_i$。

## 输出格式

输出最小和值。

## 输入输出样例 #1

### 输入 #1

```
9 7
3 0 2 5 5 3 0 6 3
```

### 输出 #1

```
11
```

## 输入输出样例 #2

### 输入 #2

```
1 10
4
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
20 20
18 16 15 9 8 8 17 1 3 17 11 9 12 11 7 3 2 14 3 12
```

### 输出 #3

```
99
```

## 说明/提示

$1 \le n \le 2 \times 10^5$

$2 \le m \le 10^9$

保证 $0 \le a_i < m$。