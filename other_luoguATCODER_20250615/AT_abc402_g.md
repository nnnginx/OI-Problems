# AT_abc402_g [ABC402G] Sum of Prod of Mod of Linear

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc402/tasks/abc402_g

给定整数 $N,M,A,B_1,B_2$。

请计算以下表达式的值：
$$ \sum_{k=0}^{N-1} \left\lbrace (Ak+B_1) \bmod M \right\rbrace \left\lbrace (Ak+B_2) \bmod M \right\rbrace $$

共有 $T$ 个测试用例，请对每个测试用例分别给出答案。

## 输入格式

输入通过标准输入给出，格式如下：

> $T$  
> $\text{case}_1$  
> $\text{case}_2$  
> $\vdots$  
> $\text{case}_T$

其中，$\text{case}_i$ 表示第 $i$ 个测试用例。

每个测试用例的格式如下：

> $N$ $M$ $A$ $B_1$ $B_2$

## 输出格式

输出 $T$ 行。第 $i$ 行输出第 $i$ 个测试用例的答案。

## 输入输出样例 #1

### 输入 #1

```
5
4 7 2 1 4
12 15 2 8 7
777 1 0 0 0
100 101 0 100 100
402 402 4 19 256
```

### 输出 #1

```
27
866
0
1000000
13728568
```

## 说明/提示

### 约束条件

- $1 \leq T \leq 10^5$
- $1 \leq N \leq 10^6$
- $1 \leq M \leq 10^6$
- $0 \leq A,B_1,B_2 < M$
- 输入中的所有数值均为整数

### 样例解释 1

对于第一个测试用例：
- 当 $k=0$ 时：$(2 \times 0 + 1) \bmod 7 = 1$，$(2 \times 0 + 4) \bmod 7 = 4$
- 当 $k=1$ 时：$(2 \times 1 + 1) \bmod 7 = 3$，$(2 \times 1 + 4) \bmod 7 = 6$
- 当 $k=2$ 时：$(2 \times 2 + 1) \bmod 7 = 5$，$(2 \times 2 + 4) \bmod 7 = 1$
- 当 $k=3$ 时：$(2 \times 3 + 1) \bmod 7 = 0$，$(2 \times 3 + 4) \bmod 7 = 3$

因此，所求值为 $1 \times 4 + 3 \times 6 + 5 \times 1 + 0 \times 3 = 27$。所以第一行输出 27。

翻译由 DeepSeek V3 完成