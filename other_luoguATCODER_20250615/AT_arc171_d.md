# AT_arc171_d [ARC171D] Rolling Hash

## 题目描述

给定整数 $P,B$ 满足 $P$ 是质数，$1\le B\le P-1$。

对于序列 $X=(x_1,x_2,\cdots,x_n)$，定义 $\operatorname{hash}(X)$ 的值为
$$\operatorname{hash}(X)=\left(\sum_{i=1}^nx_iB^{n-i}\right)\bmod P$$

给定 $M$ 对整数 $(L_i,R_i)(1\le i\le M)$，请问是否存在长度为 $N$ 的序列 $A=(A_1,A_2,\cdots,A_N)$ 满足：

- 对每一个 $i(1\le i\le M)$，都有
  $$\operatorname{hash}((A_{L_i},A_{L_i+1},\cdots,A_{R_i}))\not=0$$

## 输入格式

第一行四个整数 $P,B,N,M$，接下来 $M$ 行每行两个整数 $L_i,R_i$。

## 输出格式

若存在 $A$ 满足要求输出 `Yes`，否则输出 `No`。

### 样例 1 解释

序列 $A=(2,0,4)$ 满足要求。其中

- $\operatorname{hash}((A_1))=2$
- $\operatorname{hash}((A_1,A_2))=1$
- $\operatorname{hash}((A_2,A_3))=1$

## 输入输出样例 #1

### 输入 #1

```
3 2 3 3
1 1
1 2
2 3
```

### 输出 #1

```
Yes
```

## 输入输出样例 #2

### 输入 #2

```
2 1 3 3
1 1
2 3
1 3
```

### 输出 #2

```
No
```

## 输入输出样例 #3

### 输入 #3

```
998244353 986061415 6 11
1 5
2 2
2 5
2 6
3 4
3 5
3 6
4 4
4 5
4 6
5 6
```

### 输出 #3

```
Yes
```

## 说明/提示

-   $2 \leq P \leq 10^9$
-   $P$ 是质数。
-   $1 \leq B \leq P - 1$
-   $1 \leq N \leq 16$
-   $1 \leq M \leq \frac{N(N+1)}{2}$
-   $1 \leq L_i \leq R_i \leq N$
-   $(L_i, R_i) \neq (L_j, R_j)$ if $i \neq j$.
-   所有的输入都是整数。