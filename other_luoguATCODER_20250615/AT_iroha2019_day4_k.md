# AT_iroha2019_day4_k 世界線

## 题目描述

给定一个初始值 $N$ 和目标序列 $p_1,p_2,...p_N$，其中目标序列 $p_1,p_2,...,p_N$ 是 $1,2,...,N$ 的一个排列。初始序列只有一个数 $N$ 。对初始序列重复进行如下操作获得目标序列。求从初始序列开始创建目标序列的方法种类数，并输出其对 $1e9+7$ 取模后的值。
> 选择序列中的一个元素，在该元素和其右侧元素的中间插入一个比该元素小的数。

## 输入格式

> 第一行为整数 $N$
> 第二行为目标序列 $p_1,p_2,...p_N$

## 输出格式

> 一个整数，为从初始序列获得目标序列的方法种类数

## 输入输出样例 #1

### 输入 #1

```
4
4 2 3 1
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
4
4 3 2 1
```

### 输出 #2

```
6
```

## 输入输出样例 #3

### 输入 #3

```
7
7 6 3 4 1 2 5
```

### 输出 #3

```
36
```

## 输入输出样例 #4

### 输入 #4

```
30
30 4 26 15 21 19 14 8 12 7 16 20 2 5 25 13 3 23 18 29 10 27 1 28 9 6 11 24 22 17
```

### 输出 #4

```
321470237
```

## 说明/提示

* 输入均为整数
* $1\le N \le 2\times10^5$
* $p_1=N$
* $p_1,p_2,...p_N$为$1,2,...,N$的一个排列

#### 测试用例解说
##### 测试用例1
生成该序列的方法有以下三种，故输出 $3$
* `4 -> 4,3 -> 4,2,3 -> 4,2,3,1`
* `4 -> 4,3 -> 4,3,1 -> 4,2,3,1`
* `4 -> 4,1 -> 4,3,1 -> 4,2,3,1`