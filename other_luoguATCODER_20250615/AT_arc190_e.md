# AT_arc190_e [ARC190E] Gaps of 1 or 2

## 题目描述

给定一个长度为 N 的非负整数序列 $A=(A_1,…,A_N)$，需要回答 $Q$ 个查询。

对于第 $i$ 个查询，给定满足 $1≤L_i≤R_i≤N$ 的整数 $L_i$和 $ R_i$，考虑长度为 $R_i−L_i+1$ 的子序列 $B=(A_{L_i},…,A_{R_i}$)。
对于子序列 $B$，考虑重复执行以下操作：
1. 选择满足 $1≤i,j≤∣B∣$ 且 $1≤B_i,B_j$且$1≤j−i≤2$的整数 $i$ 和 $j$。
2. 从 $B_i$ 和 $B_j$ 中各减去 $1$。

求出可以执行操作的最大次数。

## 输入格式

输入来自标准输入，格式如下：

$
N \hspace{0.2cm} Q\\
A_1\hspace{0.2cm}⋯ \hspace{0.2cm}A_N\\
L_1\hspace{0.2cm}R_1\\
⋮\\
L_Q\hspace{0.2cm}R_Q
$

## 输出格式

请输出$Q$行。

第$i$行输出对于子序列 $B=(A_{L_i},…,A_{R_i} )$ 可以执行操作的最大次数。
### 【样例组】
#### 输入1
```
6 1
1 1 4 0 3 2
1 6
```
#### 输出1
```
5
```
#### 输入2
```
6 6
49 83 10 77 21 62
1 1
1 2
1 3
3 5
1 6
5 6
```
#### 输出2
```
0
49
59
31
151
21
```
### 【样例解释】

在这个示例中，我们求解的问题是对于给定的序列 B=(1,1,4,0,3,2)，我们可以执行以下五项操作：  
1. 选择 $i=1$ 和 $j=3$。然后，将 $B_i$ 和 $B_j$ 各减去 $1$，得到 $B=(0,1,3,0,3,2)$。
2. 选择 $i=2$ 和 $j=3$。然后，将 $B_i$ 和 $B_j$ 各减去 $1$，得到 $B=(0,0,2,0,3,2)$。
3. 选择 $i=3$ 和 $j=5$。然后，将 $B_i$ 和 $B_j$ 各减去 $1$，得到 $B=(0,0,1,0,2,2)$。
4. 选择 $i=5$ 和 $j=6$。然后，将 $B_i$ 和 $B_j$ 各减去 $1$，得到 $B=(0,0,1,0,1,1)$。
5. 选择 $i=5$ 和 $j=6$。然后，将 $B_i$ 和 $B_j$ 各减去 $1$，得到 $B=(0,0,1,0,0,0)$。

因此，可以执行操作的最大次数是5。

## 输入输出样例 #1

### 输入 #1

```
6 1
1 1 4 0 3 2
1 6
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
6 6
49 83 10 77 21 62
1 1
1 2
1 3
3 5
1 6
5 6
```

### 输出 #2

```
0
49
59
31
151
21
```

## 说明/提示

$
1≤N≤200000\\
1≤Q≤200000\\
0≤A_i≤10^9\\
1≤L_i≤R_i≤N\\
$
所有输入值均为整数。