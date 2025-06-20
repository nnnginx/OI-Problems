# AT_aising2019_e Attack to a Tree

## 题目描述

一棵有 $N$ 个节点的树，节点编号 $1$ 到 $N$。$(N-1)$ 条边中的第 $i$ 条连接节点 $U_i$ 和节点 $V_i$。点 $v$ 有非零点权 $A_v$。

现在要删去一部分边，使得各个连通块均满足以下两个条件之一：

- 连通块内点的点权均为正数；
- 连通块内点的点权和为负数。

请求出删去的边数的最小值。

## 输入格式

第一行输入单个整数 $N$。

第二行输入 $N$ 个整数，依次表示 $A_1$ 到 $A_N$。

最后 $(N-1)$ 行，第 $i$ 行输入两个整数 $U_i$ 和 $V_i$。

## 输出格式

一行一个整数表示答案。

## 输入输出样例 #1

### 输入 #1

```
7
-2 7 5 6 -8 3 4
1 2
2 3
2 4
1 5
5 6
5 7
```

### 输出 #1

```
1
```

## 输入输出样例 #2

### 输入 #2

```
4
1 2 3 4
1 2
1 3
1 4
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
6
10 -1 10 -1 10 -1
1 2
2 3
3 4
4 5
5 6
```

### 输出 #3

```
5
```

## 输入输出样例 #4

### 输入 #4

```
8
-2 3 6 -2 -2 -5 3 2
3 4
7 6
6 2
8 2
5 3
1 8
3 7
```

### 输出 #4

```
3
```

## 输入输出样例 #5

### 输入 #5

```
10
3 4 9 6 1 5 -1 10 -10 -10
7 4
5 6
8 1
9 5
7 1
10 3
2 8
4 10
9 2
```

### 输出 #5

```
3
```

## 说明/提示

#### 样例 #1 解释

切断第 $1,2$ 条边即可。

#### 数据规模与约定

对于全部测试数据，保证：

- $1\le N\le 5000$；
- 当 $1\le i\le N$ 时，$1\le |A_i|\le 10^9$。
- 当 $1\le i\le N-1$ 时，$1\le U_i,V_i\le N$，$U_i\neq V_i$。