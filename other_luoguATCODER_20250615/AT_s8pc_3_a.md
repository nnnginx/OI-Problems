# AT_s8pc_3_a カレンダー

## 题目描述

有一张有n行、7列的日历表，其中第一天在第一列。

请从这张表中找出一个3 * 3的子表，要求表中9个数的和除以11的余数为k。

数据范围： 1<=n<=10^9， 0<=k<=10

输入一行：n k

输出：有多少张符合条件的子表。

样例一：

母表（7行）：

1	2	3	4	5	6	7

8	9	10	11	12	13	14

15	16	17	18	19	20	21

22	23	24	25	26	27	28

29	30	31	32	33	34	35

36	37	38	39	40	41	42

43	44	45	46	47	48	49

符合条件的子表（2张）：

5	6	7

12	13	14

19	20	21

16	17	18

23	24	25

30	31	32

## 输入格式

仅一行N,K

## 输出格式

满足条件3\3×3正方形的放置方法的次数输出一行。
但是,如果一个条件都无法满足,则输出为0.

## 输入输出样例 #1

### 输入 #1

```
7 7
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
6 0
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```

```

### 输出 #3

```
7
```

## 输入输出样例 #4

### 输入 #4

```

```

### 输出 #4

```
45
```