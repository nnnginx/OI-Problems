# AT_nomura2020_f Sorting Game

## 题目描述

高桥君和须贺君想出了一个基于数列的游戏。游戏规则如下：


首先准备一个长度为 $M$ 的数列 $a = a_1, a_2, ..., a_M$，其中每个元素都是 $0$ 到 $2^N-1$ 之间的整数。

接下来，须贺君可以任意多次进行以下操作：

选择一个正整数 $d$，并将 $a$ 中每个元素的二进制表示的第 $d$ 位（最低位为第 $1$ 位）设为 $0$。



最终，高桥君可以任意多次进行以下操作，以尝试将 $a$ 排序：

选择相邻的两个元素 $a_i$ 和 $a_{i+1}$，若它们的二进制表示恰好有一位不同，则交换 $a_i$ 和 $a_{i+1}$。
已知存在 $2^{NM}$ 种满足条件的长度为 $M$ 的数列 $a$。其中须贺君无论如何进行操作，高桥君都可以通过合适的交换将 $a$ 排序。请将结果对 $10^9+7$ 取模后输出。

## 输入格式

输入共一行，包含两个整数 $N$ 和 $M$。

## 输出格式

输出一个整数，表示可以通过合适的交换将数列 $a$ 排序的数列 $a$ 的数量对 $10^9+7$ 取模后的结果。
翻译贡献：Lord_Sky2048

## 输入输出样例 #1

### 输入 #1

```
2 5
```

### 输出 #1

```
352
```

## 输入输出样例 #2

### 输入 #2

```
2020 530
```

### 输出 #2

```
823277409
```