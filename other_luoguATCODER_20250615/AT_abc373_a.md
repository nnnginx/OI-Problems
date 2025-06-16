# AT_abc373_a [ABC373A] September

## 题目描述

### 问题描述

有 $12$ 个由小写英文字母组成的字符串 $S_1, S_2, \ldots, S_{12}$ 。

求有多少个 $S_i$ 的长度恰好为 $i$ 。

## 输入格式

$12$ 行，每行一个字符串 $S_i$。

## 输出格式

一个数，表示答案。

## 输入输出样例 #1

### 输入 #1

```
january
february
march
april
may
june
july
august
september
october
november
december
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
ve
inrtfa
npccxva
djiq
lmbkktngaovl
mlfiv
fmbvcmuxuwggfq
qgmtwxmb
jii
ts
bfxrvs
eqvy
```

### 输出 #2

```
2
```

## 说明/提示

#### 数据限制

> - 每个 $S_i$ 的长度都在 $1 \sim 100$ 之间。

#### 样例解析

> - 对于样例 $1$ ，只有 $i = 9$ 的情况下， $S_i$ 长度为 $i$ 。所以输出 `1` 。
> - 对于样例 $2$ ，在 $i = 4$ 和 $i = 8$ 的情况下， $S_i$ 长度为 $i$ 。所以输出 `2` 。