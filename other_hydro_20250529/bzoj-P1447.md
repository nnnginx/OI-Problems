## 题目描述

After he partitioned his farm into $r$ rows and $c$ squares conveniently labeled $(1,1)$ through $(r,c)$, Farmer John spent days cutting the hay and stacking a huge amount of it in square $(1,1)$. He then undertook the task of mapping out the $n$ haypaths through the farm so that he could deduce the maximum rate he could move hay from square $(1,1)$ to square $(r,c)$. Each haypath uniquely connects the middle of two rectilinearly adjacent partitioned squares and has some capacity limit $l_i$ that is the maximum amount of hay that can be transported in either direction across the haypath. He's just positive that he can move hay at a reasonable rate to the other side of the farm but he doesn't know what the fastest rate is. Help him learn it.

## 输入格式

Line $1$: Three separated integers: $r,c$, and $n$ 

Lines $2\cdots n+1$: Line $i+1$ describes path $i$ with five space-separated integers: $r_1,c_1,r_2,c_2,l_i$ which denote a haypath connecting $(r1,c1)$ to $(r2,c2)$ with capacity $l_i$.

## 输出格式

Line $1$: One number, on a line by itself, the maximum amount of material which can be transported from $(1,1)$ to $(r,c)$ simultaneously.

```input1
3 3 8
1 1 1 2 5
1 1 2 1 3
1 2 2 2 5
2 1 2 2 2
2 2 2 3 1
2 2 3 2 6
2 3 3 3 4
3 2 3 3 7
```

```output1
7
```

## 样例解释

The grid is as follows:

```
*--5--* . . *
|     |     
3     5     :
|     |    
*--2--*--1--*
      |     |
:     6     4
      |     |
* . . *--7--*
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq r,c\leq 200$，$1\leq n\leq 8\times 10^4$，$1\leq l_i\leq 2\times 10^7$。

