# AT_asaporo_d ストラックアウト

## 题目描述

高桥君家里有一排长为 $N$ 的面板，编号依次为 $1, 2, \ldots, N$。每个面板 $i$ 上都有一个数字 $A_i$，他通过向这些面板投球来进行游戏。

高桥君总共投了 $K$ 次球。当第 $i$ 次投中的面板是面板 $p_i$ 时，游戏的得分为 $\sum_{i=1}^{K} i \times A_{p_i}$。

不幸的是，高桥君投完球后忘记了他投中的面板序号 $p_1, p_2, \ldots, p_K$。他只记得每次投的球都满足一个规则：对于 $1 \leq i \leq K-1$，都有 $1 \leq p_{i+1} - p_i \leq M$。请帮助高桥君计算出在这种条件下他可能获得的最大得分。

## 输入格式

输入数据从标准输入给出，格式如下：

> $N$ $M$ $K$ $A_1$ $A_2$ $\ldots$ $A_N$

## 输出格式

输出高桥君可能获得的最大得分。

## 输入输出样例 #1

### 输入 #1

```
5 2 3
10 2 8 10 2
```

### 输出 #1

```
56
```

## 输入输出样例 #2

### 输入 #2

```
5 5 2
5 2 10 5 9
```

### 输出 #2

```
28
```

## 输入输出样例 #3

### 输入 #3

```
10 3 5
3 7 2 6 9 4 8 5 1 1000000000
```

### 输出 #3

```
5000000078
```

## 说明/提示

### 约束
- $1 \leq M \leq N \leq 10^5$
- $1 \leq K \leq \min(300, N)$
- $1 \leq A_i \leq 10^9$

### 部分得分
- 对于 100 分的数据，满足 $M = N$。
- 对于 200 分的数据，满足 $N \leq 300$ 且 $K \leq 30$。
- 对于 300 分的数据，满足 $K \leq 30$。

### 样例解释 1
按照顺序投向面板 $1, 3, 4$ 时，得分可以达到最大。

### 样例解释 2
此输入满足 $M = N$ 的部分得分情况。

 **本翻译由 AI 自动生成**