# AT_arc060_a [ABC044C] 高橋君とカード（高桥和卡片）

## 题目描述

高桥有 $n$ 张卡片，在第 $i$ 张卡片上面写着整数 $x_i$。

高桥从这些卡片中挑选一张或更多卡片，要求选择的卡片上整数的平均数等于 $A$。求有几种方案。

**两张卡片即使数字相同也被看作是不同的两张卡片。**

## 输入格式

第 $1$ 行有两个整数 $N,A$，以空格隔开，表示卡片个数和要求的平均数。

第 $2$ 行 $N$ 个整数 $x_i$，以空格隔开，表示第 $i$ 张卡片上的整数。

## 输出格式

一个整数，表示总的方案数。

## 输入输出样例 #1

### 输入 #1

```
4 8
7 9 8 9
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
3 8
6 6 9
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
8 5
3 6 2 8 7 6 5 9
```

### 输出 #3

```
19
```

## 输入输出样例 #4

### 输入 #4

```
33 3
3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3 3
```

### 输出 #4

```
8589934591
```

## 说明/提示

### 数据规模与约定
* 对于 $200$ 分的数据，$1\le N,A,x_i\le16$ 且均为整数。
* 对于 $300$ 分（满分）的数据，$1\le N,A,x_i\le50$ 且均为整数。

### 样例解释 1
你共有如下 $5$ 种方案使平均数为 $8$：
* 选第 $3$ 张。
* 选第 $1,2$ 张。
* 选第 $1,4$ 张。
* 选第 $1,2,3$ 张。
* 选第 $1,3,4$ 张。

### 样例解释 4
不保证答案在 $32$ 位有符号整数范围内。

题目原文由 [Stephzzz](https://www.luogu.com.cn/user/71988) 翻译，其他部分由 [Ascnbeta](https://www.luogu.com.cn/user/767561) 补充。