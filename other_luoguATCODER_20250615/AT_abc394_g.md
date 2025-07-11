# AT_abc394_g [ABC394G] Dense Buildings

## 题目描述

[problemUrl]: https://atcoder.jp/contests/abc394/tasks/abc394_g

在东西南北方向被划分为 $H \times W$ 个区域的街区中，每个区域恰好建有一座大楼。  
具体来说，北起第 $i$ 行（$1 \leq i \leq H$）西起第 $j$ 列（$1 \leq j \leq W$）的区域（以下简称区域 $(i,j)$）建有一座 $F_{i,j}$ 层的大楼。

高桥君有两种移动方式。当他在区域 $(i,j)$ 大楼的 $X$ 层（$1 \leq X \leq F_{i,j}$）时，可以进行以下移动：

- 通过**楼梯**在同一大楼内移动到相邻的上一层或下一层。但无法从 $1$ 层移动到更下层，也无法从 $F_{i,j}$ 层移动到更上层。
- 通过 **（高空）通道** 移动到东西南北相邻区域中某座高度至少为 $X$ 层的大楼的 $X$ 层。

此处，区域 $(i,j)$ 与区域 $(i',j')$ 东西南北相邻的定义为 $\lvert i - i' \rvert + \lvert j - j' \rvert = 1$。

请回答 $Q$ 个查询。第 $i$ 个（$1 \leq i \leq Q$）查询内容如下：

> 请求出高桥君从区域 $(A_i, B_i)$ 大楼的 $Y_i$ 层移动到区域 $(C_i, D_i)$ 大楼的 $Z_i$ 层时，**楼梯**使用次数的最小可能值。  
> 注意：每次上下移动一层均计为一次楼梯使用（例如从某大楼 $1$ 层移动到 $6$ 层需使用 $5$ 次楼梯）。  
> 同时，通道使用次数无需最小化。

## 输入格式

输入通过标准输入按以下格式给出：

> $H$ $W$  
> $F_{1,1}$ $F_{1,2}$ $\ldots$ $F_{1,W}$  
> $F_{2,1}$ $F_{2,2}$ $\ldots$ $F_{2,W}$  
> $\vdots$  
> $F_{H,1}$ $F_{H,2}$ $\ldots$ $F_{H,W}$  
> $Q$  
> $A_1$ $B_1$ $Y_1$ $C_1$ $D_1$ $Z_1$  
> $A_2$ $B_2$ $Y_2$ $C_2$ $D_2$ $Z_2$  
> $\vdots$  
> $A_Q$ $B_Q$ $Y_Q$ $C_Q$ $D_Q$ $Z_Q$

## 输出格式

输出 $Q$ 行。第 $i$ 行输出第 $i$ 个查询的答案。

## 输入输出样例 #1

### 输入 #1

```
3 3
12 10 6
1 1 3
8 6 7
2
1 1 10 3 1 6
1 1 6 1 2 4
```

### 输出 #1

```
10
2
```

## 说明/提示

### 约束条件

- $1 \leq H \leq 500$
- $1 \leq W \leq 500$
- $1 \leq F_{i,j} \leq 10^6$
- $1 \leq Q \leq 2 \times 10^5$
- $1 \leq A_i, C_i \leq H$
- $1 \leq B_i, D_i \leq W$
- $1 \leq Y_i \leq F_{A_i,B_i}$
- $1 \leq Z_i \leq F_{C_i,D_i}$
- $(A_i, B_i, Y_i) \neq (C_i, D_i, Z_i)$
- 所有输入均为整数

### 样例解释 1

对于第 $1$ 个查询，以下移动方式共使用 $10$ 次楼梯：
- 通过通道从区域 $(1,1)$ 大楼 $10$ 层移动到区域 $(1,2)$ 大楼 $10$ 层
- 使用 $4$ 次楼梯从 $10$ 层下到 $6$ 层
- 通过通道移动到区域 $(1,3)$ 大楼 $6$ 层
- 使用 $3$ 次楼梯下到 $3$ 层
- 通过通道移动到区域 $(2,3)$ 大楼 $3$ 层
- 通过通道移动到区域 $(3,3)$ 大楼 $3$ 层
- 使用 $3$ 次楼梯上到 $6$ 层
- 通过通道移动到区域 $(3,2)$ 大楼 $6$ 层
- 通过通道移动到区域 $(3,1)$ 大楼 $6$ 层  
由于无法用 $9$ 次或更少楼梯完成移动，故输出 $10$。

对于第 $2$ 个查询，通过通道移动到区域 $(1,2)$ 大楼后，使用 $2$ 次楼梯从 $6$ 层下到 $4$ 层即可完成移动，故输出 $2$。

翻译由 DeepSeek R1 完成