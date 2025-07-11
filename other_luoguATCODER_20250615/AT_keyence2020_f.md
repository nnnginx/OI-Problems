# AT_keyence2020_f Monochromization

## 题目描述

我们有一个$H \times W$的网格，每个正方形都被涂成黑色或白色。

给定字符串$A_1,A_2,...,A_H$，表示初始每一个正方形的颜色。$A_i$的第$j$个字符表示$(i,j)$的颜色。“$.$”表示白色，“$#$”表示黑色。

规定以下几种操作：

1. 选择一行，然后将该行中的所有正方形涂成白色。

2. 选择一行，然后将该行中的所有正方形涂成黑色。

3. 选择一列，然后将该列中的所有正方形白色。

4. 选择一列，然后将该列中的所有正方形涂成黑色。

试求在将网格涂色的$2^{HW}$种方法中，通过以任何顺序执行任何次数操作，可以从初始状态获得多少种不同的结果？结果对$998244353$取模。

## 输入格式

第一行输入两个数$H,W$，后面$H$行分别输入$A_1,A_2,...,A_H$。

## 输出格式

一行，直接输出答案。

## 输入输出样例 #1

### 输入 #1

```
2 2
#.
.#
```

### 输出 #1

```
15
```

## 输入输出样例 #2

### 输入 #2

```
3 3
...
...
...
```

### 输出 #2

```
230
```

## 输入输出样例 #3

### 输入 #3

```
2 4
#...
...#
```

### 输出 #3

```
150
```

## 输入输出样例 #4

### 输入 #4

```
6 7
.......
.......
.#.....
..#....
.#.#...
.......
```

### 输出 #4

```
203949910
```

## 说明/提示

$1≤H,W≤10$，且$H,W$为正整数。

$|A_i|=W (1≤i≤H)$，且保证$A_i$由“$.$”和“$#$”组成。