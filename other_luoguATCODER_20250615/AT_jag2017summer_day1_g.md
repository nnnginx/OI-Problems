# AT_jag2017summer_day1_g ツーリスト問題

## 题目描述

旅游者手中有两个等长的列表。

每个列表的长度为 $N$，在第 $i$ 个列表中的第 $j$ 个元素表示为 $A_{i,j}$。这里，$A_{i,j}$ 是正整数或负整数，且不为 $0$。

旅游者希望通过以下步骤调整和操作这两个列表：

- 首先，将列表中所有的负整数替换为正整数，要求原有相同的负数必须替换成相同的正数，而原来不同的负数则需要替换为不同的正数。
- 接下来，准备一张 2 行 $N$ 列的网格纸，在第 $i$ 行第 $j$ 列格子上写入第 $i$ 个列表的第 $j$ 个数。
- 最后，剪去相邻格子间填写了不同数值的边以及外边框，这样网格纸会被剪成若干块。请计算这些独立块的数量。

旅游者希望通过合适地替换负整数，将网格纸的独立块数量尽可能减少。请问最终纸会被分成多少块？

## 输入格式

输入通过标准输入给出，格式如下：

> $N$ $A_{1,1}$ $A_{1,2}$ $...$ $A_{1,N}$ $A_{2,1}$ $A_{2,2}$ $...$ $A_{2,N}$

## 输出格式

输出纸被分割成的独立块数量。

## 输入输出样例 #1

### 输入 #1

```
5
1 2 1 2 1
-1 -2 -3 -3 -3
```

### 输出 #1

```
5
```

## 输入输出样例 #2

### 输入 #2

```
15
1 -1 1 -1 -1 -2 2 -1 3 3 3 -3 -2 -2 1
2 -1 1 1 -1 -2 -1 2 -2 3 3 -2 -2 -2 3
```

### 输出 #2

```
9
```

## 说明/提示

- $1 \le N \le 10^5$
- $1 \le |A_{i,j}| \le 300$

### 样例解释

例如，若将 $-1$ 替换为 $999$，$-2$ 替换为 $2$，$-3$ 替换为 $1$，可以得到如附图所示的结果，此时纸块被分成最少的 $5$ 块。  
![92e7ebbff942cc1af02ea1a3e5aa7a75.png](https://img.atcoder.jp/jag2017summer-day1/92e7ebbff942cc1af02ea1a3e5aa7a75.png)

 **本翻译由 AI 自动生成**