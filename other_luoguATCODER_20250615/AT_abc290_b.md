# AT_abc290_b [ABC290B] Qual B

## 题目描述

在一场比赛中，有 $N$ 个参赛者，所有参赛者都有一个排名。

有一个长度为 $N$ 的字符串 $S$，代表参赛者是否想参加决赛。

- 如果第 $i$ 个字符为 `o`，表示排名第 $i$ 的参赛者要参加决赛；
- 如果第 $i$ 个字符为 `x`，表示排名第 $i$ 的参赛者不要参加决赛；

在要参加决赛的参赛者中，排名前 $K$ 的可以参加决赛。

输出满足以下条件的长度为 $N$ 的字符串 $T$：

- 如果第 $i$ 名参赛者可以参加决赛，则第 $i$ 个字符为 `o`；
- 如果第 $i$ 名参赛者不可以参加决赛，则第 $i$ 个字符为 `x`；

## 输入格式

输入以以下格式：

>$N\ K$
>
>$S$

## 输出格式

输出答案。

## 输入输出样例 #1

### 输入 #1

```
10 3
oxxoxooxox
```

### 输出 #1

```
oxxoxoxxxx
```

## 说明/提示

- $N,K$ 都是整数
- $1\leq K \leq N \leq100$
- $S$ 是一个长度为 $N$ 并且由 `o` 和 `x` 组成的字符串
- $S$ 至少有 $K$ 个 `o`