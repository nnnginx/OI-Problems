## 题目描述

为保证会场安全，专家确定了每一行每一列的保镖数，这个信息以一种压缩的形式给出。确定是否有可能实现这样一种方案，在每行每列安排确定数量的保镖。假设座位最初都是空的，也就是说保安可以被安排在任意一个座位上。 题目等价于已知一个 $01$ 矩阵的每行、每列各有多少个 $1$，问这样的矩阵是否存在。

输入数据归纳为：有 $r$ 个正整数对 $a_1,b_1,a_2,b_2, \ldots a_r,b_r$ 表示这个 $01$ 矩阵一共有 $b_1+b_2+ \ldots +b_r$ 行，其中有 $b_i$ 个行都含有 $a_i$ 个 $1$。 同样的，有 $c$ 个正整数对 $p_i$ 和 $q_i$ 来表示列的信 息。

## 输入格式

The input begins with the description of the rows. The first line of the input contains one positive integer $r$ : the number of groups of rows. $r$ lines follow. Each of these lines contains $2$ positive integers: the required number of bodyguards in each row of the group and the number of rows that form the group. This is followed by the description of column groups. The next line contains one positive integer $c$ : the number of groups of columns. $c$ lines follow. Each of these lines contains $2$ positive integers: the required number of bodyguards in each column of the group and the number of columns that form the group.

## 输出格式

Output a single line with the number `1` if the constraints are satisfiable and the number `0` otherwise.

```input1
2
2 1
1 2
1
2 2
```
```output1
1
```

## 样例说明 1
There are two groups of rows: the first one has one row that must contain two bodyguards, the second one has two rows that must contain one bodyguard each. There is one group of columns: each of the two columns must contain two bodyguards. One possible placement of bodyguards:

```
 XX
 X.
 .X
```

```input2
2
3 2
1 1
2
3 2
1 1
```
```output2
0
```

## 样例说明 2

Two of the rows are required to be full of bodyguards. Hence there must be at least two bodyguards in each column. However, the last column must only contain one bodyguard, which is a contradiction.

## 数据规模与约定

对于 $50\%$ 的数据，$r,c\le 2\times10^3$，最多有 $10^6$ 名保镖。

对于 $100\%$ 的数据，保镖总数最多为 $10^{18}$，所有数字均为正整数，且不超过 $10^9$，$1\le r,c\le 2\times 10^5$。数据保证按行和按列计算的总保镖数相等。