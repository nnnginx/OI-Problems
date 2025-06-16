# AT_arc190_d [ARC190D] Matrix Pow Sum

## 题目描述

给定素数 $p$ 和一个 $N \times N$ 的矩阵 $A = (A_{i,j})$（$1 \leq i,j \leq N$），其中每个元素 $A_{i,j}$ 是 $0$ 到 $p-1$ 之间的整数。  

定义矩阵 $B$ 为将 $A$ 中所有 $0$ 替换为 $1$ 到 $p-1$ 之间的整数后得到的矩阵。设 $A$ 中 $0$ 的个数为 $K$，则共有 $(p-1)^K$ 种可能的 $B$。  

要求计算所有可能的 $B$ 对应的 $B^p$（矩阵的 $p$ 次幂）之和，并将每个元素对 $p$ 取模后输出。

## 输入格式

输入格式如下：  
> $N$ $p$  
> $A_{1,1}$ $\cdots$ $A_{1,N}$  
> $\vdots$  
> $A_{N,1}$ $\cdots$ $A_{N,N}$

## 输出格式

输出 $N$ 行，每行包含 $N$ 个整数。第 $i$ 行第 $j$ 列表示所有 $B^p$ 之和的 $(i,j)$ 元素对 $p$ 取模后的结果，整数间以空格分隔。

## 输入输出样例 #1

### 输入 #1

```
2 3
0 1
0 2
```

### 输出 #1

```
0 2
1 2
```

## 输入输出样例 #2

### 输入 #2

```
3 2
1 0 0
0 1 0
0 0 1
```

### 输出 #2

```
1 1 1
1 1 1
1 1 1
```

## 输入输出样例 #3

### 输入 #3

```
4 13
0 1 2 0
3 4 0 5
0 6 0 7
8 9 0 0
```

### 输出 #3

```
8 0 6 5
11 1 8 5
8 0 4 12
8 0 1 9
```

## 说明/提示

### 约束条件  
- $1 \leq N \leq 100$  
- $p$ 是满足 $1 \leq p \leq 10^9$ 的素数  
- $0 \leq A_{i,j} \leq p-1$  
- 输入均为整数  

### 样例解释 1  
所有可能的 $B$ 对应的 $B^3$ 如下：  
- $\begin{pmatrix}1 & 1 \\ 1 & 2\end{pmatrix}^3 = \begin{pmatrix}5 & 8 \\ 8 & 13\end{pmatrix}$  
- $\begin{pmatrix}1 & 1 \\ 2 & 2\end{pmatrix}^3 = \begin{pmatrix}9 & 9 \\ 18 & 18\end{pmatrix}$  
- $\begin{pmatrix}2 & 1 \\ 1 & 2\end{pmatrix}^3 = \begin{pmatrix}14 & 13 \\ 13 & 14\end{pmatrix}$  
- $\begin{pmatrix}2 & 1 \\ 2 & 2\end{pmatrix}^3 = \begin{pmatrix}20 & 14 \\ 28 & 20\end{pmatrix}$  
总和为 $\begin{pmatrix}48 & 44 \\ 67 & 65\end{pmatrix}$，各元素对 $p=3$ 取模后输出。  

### 样例解释 2  
所有可能的 $B$ 对应的 $B^2$ 为：  
- $\begin{pmatrix}1 & 1 & 1 \\ 1 & 1 & 1 \\ 1 & 1 & 1\end{pmatrix}^2 = \begin{pmatrix}3 & 3 & 3 \\ 3 & 3 & 3 \\ 3 & 3 & 3\end{pmatrix}$  
总和对 $p=2$ 取模后输出。  

翻译由 DeepSeek R1 完成