# AT_arc057_d [ARC057D] 全域木

## 题目描述

给定 $N-1$ 个数 $A_1,A_2,\dots,A_{N-1}$ ，求满足其最小生成树边权升序排列为序列 $\{A\}$ ，且所有边权为 $1$ 到 $\frac{N\times(N-1)}{2}$ 的排列的 $N$ 阶完全图数量。  
答案对 $10^9+7$ 取模。

## 输入格式

输入第一行为一个整数 $N$ ，接下来 $N-1$ 行，每行一个整数 $A_i$ ，意义如题目所述。

## 输出格式

输出一个整数，表示所求完全图数量对 $10^9+7$ 取模的结果。

## 输入输出样例 #1

### 输入 #1

```
3
1
2
```

### 输出 #1

```
6
```

## 输入输出样例 #2

### 输入 #2

```
5
1
2
4
6
```

### 输出 #2

```
69120
```

## 输入输出样例 #3

### 输入 #3

```
5
2
3
4
5
```

### 输出 #3

```
0
```

## 输入输出样例 #4

### 输入 #4

```
10
1
2
4
6
8
10
11
12
14
```

### 输出 #4

```
837872061
```

## 说明/提示

$1 \leq N \leq 30$  
$1 \leq A_i \leq \frac{N\times(N-1)}{2}$  
保证 $A_i$ 两两不同。