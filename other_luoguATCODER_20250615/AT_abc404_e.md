# AT_abc404_e 茶碗和豆子

## 题目描述

你有 $N$ 个茶碗，它们排成一排，从左往右依次编号 $0,1,\cdots,N-1$。

对于 $1$ 号碗和它右边的碗，$i$ 号碗上面写有一个数字 $C_i$，里面装有 $A_i$ 颗豆子；$0$ 号碗上面没有数字，碗里没有豆子。

你将执行以下操作若干次：
- 选择一个带有数字的、装有豆子的碗 $i$，拿走其中的一部分豆子（可以全拿）；
- 将你拿出的豆子任意放入 $i-C_i,i-C_i+1,\cdots,i-1$ 号碗中，你放入的豆子数总和要等于你从 $i$ 号碗中拿出的豆子数。

请你求出让所有豆子都被放入 $0$ 号碗的最小操作次数。

## 输入格式

第一行一个整数 $N(1\le N\le 2000)$。\
第二行 $N-1$ 个整数 $C_1,C_2,\cdots,C_{N-1}(1\le C_i\le i)$。\
第三行 $N-1$ 个整数 $A_1,A_2,\cdots,A_{N-1}(0\le A_i\le 1)$。

保证 $\sum\limits_{i=1}^{N-1}A_i>0$，即不会出现所有碗里都没有豆子的情况。

## 输出格式

输出一个整数表示答案。

## 输入输出样例 #1

### 输入 #1

```
5
1 1 2 1
1 0 0 1
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
6
1 2 1 3 1
1 1 0 1 1
```

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
16
1 1 1 2 5 1 1 3 4 1 4 3 1 1 2
1 0 0 0 1 0 0 1 1 0 0 0 0 0 1
```

### 输出 #3

```
7
```

## 说明/提示

**样例 1 解释**

以下是一种可能的操作序列：
- 从 $4$ 号碗里拿出 $1$ 颗豆子，将其放入 $3$ 号碗；
- 从 $3$ 号碗里拿出 $1$ 颗豆子，将其放入 $1$ 号碗；
- 从 $1$ 号碗里拿出 $2$ 颗豆子，将其放入 $0$ 号碗。

花费 $3$ 次操作完成了题目的要求。可以证明这是可能的最小操作次数。

**样例 2 解释**

以下是一种可能的操作序列：
- 从 $5$ 号碗里拿出 $1$ 颗豆子，将其放入 $4$ 号碗；
- 从 $4$ 号碗里拿出 $2$ 颗豆子，$1$ 颗放入 $1$ 号碗，$1$ 颗放入 $2$ 号碗；
- 从 $1$ 号碗里拿出 $2$ 颗豆子，将其放入 $0$ 号碗；
- 从 $2$ 号碗里拿出 $2$ 颗豆子，将其放入 $0$ 号碗。

花费 $4$ 次操作完成了题目的要求。可以证明这是可能的最小操作次数。

By chenxi2009