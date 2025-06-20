# AT_arc192_c [ARC192C] Range Sums 2

## 题目描述

[problemUrl]: https://atcoder.jp/contests/arc192/tasks/arc192_c

**本题为交互式问题。**

给定一个正整数 $N$。

Snuke 隐藏了一个由 $(1,2,\dots,N)$ 排列而成的正整数序列 $P = (P_1, P_2, \dots, P_N)$ 和一个长度为 $N$ 的正整数序列 $A = (A_1, A_2, \dots, A_N)$。**其中保证 $P_1 < P_2$。**

你可以向 Snuke 发送最多 $2N$ 次查询。每次查询的形式如下：

- 指定两个**不同**的正整数 $s, t$（$1 \leq s, t \leq N$），获得 $\displaystyle \sum_{i=\min(P_s, P_t)}^{\max(P_s, P_t)} A_i$ 的值。

请通过交互确定 $P$ 和 $A$。

### 输入输出格式

本题为交互式问题。

首先，从标准输入读取正整数 $N$：

> $N$

接下来，你可以向 Snuke 发送最多 $2N$ 次查询。每次发送查询时，按照以下格式输出（注意末尾换行）：

> ? $s$ $t$

发送查询后，Snuke 的回复将通过标准输入以下列形式给出：

> $X$

其中：
- 若 $X \neq -1$，表示 $\displaystyle \sum_{i=\min(P_s, P_t)}^{\max(P_s, P_t)} A_i = X$。
- 若 $X = -1$，表示 $s, t$ 不满足约束条件或查询次数超过 $2N$ 次。
  - 此时程序已被判定为错误，请立即终止。

当确定 $P$ 和 $A$ 后，请按照以下格式输出答案（不计入查询次数）：

> ! $P_1$ $P_2$ $\dots$ $P_N$ $A_1$ $A_2$ $\dots$ $A_N$

**特别注意 $P_1 < P_2$ 必须成立。** 输出后请立即终止程序。

若输出格式不符合上述要求，评测系统将返回：

```
-1
```

此时程序已被判定为错误，请立即终止。

## 输入格式

无

## 输出格式

无

## 说明/提示

### 约束条件

- $3 \leq N \leq 5000$
- $1 \leq P_i \leq N$（$1 \leq i \leq N$）
- $P_i \neq P_j$（$i \neq j$）
- $P_1 < P_2$
- $1 \leq A_i \leq 10^9$（$1 \leq i \leq N$）
- $N, P_i, A_i$ 均为整数
- $P$ 和 $A$ 在交互开始前已确定

### 注意事项

- **每次输出后，请确保在末尾添加换行并刷新输出缓冲区。否则可能导致 TLE。**
- 输出答案后，或在收到 `-1` 后，请立即终止程序。否则判定结果可能异常。
- 多余换行将被视为格式错误。
- **本题评测系统为非自适应的。** 即 $P$ 和 $A$ 在交互前已确定且不会改变。

### 输入输出示例

以下为 $N=6$，$P=(2,4,6,5,3,1)$，$A=(1,9,2,25,2,9)$ 时的交互示例：

| 输入（系统） | 输出（程序）               | 说明                                                                 |
|:--------------:|:----------------------------:|:----------------------------------------------------------------------:|
| `6`          |                            | 从标准输入读取 $N=6$                                                |
| `36`         | `? 1 2`                    | 发送查询 $s=1, t=2$，返回 $\sum_{i=2}^{4} A_i = 9+25+2 = 36$        |
| `27`         | `? 2 5`                    | 发送查询 $s=2, t=5$，返回 $\sum_{i=3}^{4} A_i = 2+25 = 27$      |
|              | `! 2 4 6 5 3 1 1 9 2 25 2 9` | 提交答案并终止程序                                                   |

翻译由 DeepSeek R1 完成