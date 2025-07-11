# AT_abc400_g [ABC400G] Patisserie ABC 3

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc400/tasks/abc400_g

在 ABC 西点店工作的糕点师高桥君决定为纪念 AtCoder Beginner Contest 400 推出特别蛋糕套装。

ABC 西点店销售 $N$ 种蛋糕，分别为蛋糕 $1$，蛋糕 $2$，……，蛋糕 $N$。  
每个蛋糕具有三个非负整数值属性：美观度、美味度和人气度。具体来说，蛋糕 $i$ 的美观度、美味度、人气度分别为 $X_i$，$Y_i$，$Z_i$。

高桥君计划将蛋糕无重复地组成 $K$ 对进行销售。  
形式化地说，需要选出 $2K$ 个**互不相同**的 $1$ 到 $N$ 之间的整数 $a_1, b_1, a_2, b_2, \ldots, a_K, b_K$，并将蛋糕 $a_i$ 与蛋糕 $b_i$ 组成一对。  
当蛋糕 $a_i$ 与蛋糕 $b_i$ 组成一对时，该对的价格定义为 $\max(X_{a_i} + X_{b_i},\ Y_{a_i} + Y_{b_i},\ Z_{a_i} + Z_{b_i})$。  
其中 $\max(P, Q, R)$ 表示 $P, Q, R$ 中的最大值。

请计算这 $K$ 对蛋糕价格总和的可能最大值。

给定 $T$ 个测试用例，请对每个用例输出答案。

## 输入格式

输入通过标准输入给出，格式如下：

> $T$  
> $\mathrm{case}_1$  
> $\mathrm{case}_2$  
> $\vdots$  
> $\mathrm{case}_T$

其中 $\mathrm{case}_i$ 表示第 $i$ 个测试用例，每个测试用例的格式为：

> $N$ $K$  
> $X_1$ $Y_1$ $Z_1$  
> $X_2$ $Y_2$ $Z_2$  
> $\vdots$  
> $X_N$ $Y_N$ $Z_N$

## 输出格式

输出 $T$ 行。第 $i$ 行（$1 \leq i \leq T$）应输出第 $i$ 个测试用例的答案。

## 输入输出样例 #1

### 输入 #1

```
1
3 1
6 3 8
3 5 0
2 7 3
```

### 输出 #1

```
12
```

## 输入输出样例 #2

### 输入 #2

```
2
5 2
1 2 3
1 2 3
1 2 3
1 2 3
100 100 200
6 2
21 74 25
44 71 80
46 28 96
1 74 24
81 83 16
55 31 1
```

### 输出 #2

```
209
333
```

## 说明/提示

### 约束条件

- $1 \leq T \leq 1000$
- $2 \leq N \leq 10^5$
- 对于每个输入文件，所有测试用例的 $N$ 总和不超过 $10^5$。
- $1 \leq K \leq \lfloor \frac{N}{2} \rfloor$（对于实数 $x$，$\lfloor x \rfloor$ 表示不超过 $x$ 的最大整数）。
- $0 \leq X_i, Y_i, Z_i \leq 10^9$
- 输入中的所有值均为整数

### 样例解释 1

从 $3$ 个蛋糕中选择 $1$ 对：  
- 蛋糕 $1$ 和 $2$ 组成的对价格为 $\max(6+3, 3+5, 8+0) = 9$  
- 蛋糕 $1$ 和 $3$ 组成的对价格为 $\max(6+2, 3+7, 8+3) = 11$  
- 蛋糕 $2$ 和 $3$ 组成的对价格为 $\max(3+2, 5+7, 0+3) = 12$  
因此选择蛋糕 $2$ 和 $3$ 组成的对，输出 $12$。

### 样例解释 2

注意每个蛋糕最多只能出现在一个对中。此外，即使不同种类的蛋糕，其美观度、美味度、人气度也可能完全相同。  
对于第一个测试用例，选择蛋糕 $1$ 和 $2$（价格 $6$）以及蛋糕 $3$ 和 $5$（价格 $203$），总价格为 $209$。  
对于第二个测试用例，选择蛋糕 $2$ 和 $3$（价格 $176$）以及蛋糕 $4$ 和 $5$（价格 $157$），总价格为 $333$。

翻译由 DeepSeek R1 完成