## 题目描述

给出正整数数列 $a_1,a_2,\ldots,a_n$，其中子序列 $b_1,b_2,\ldots,b_k$ 满足任取 $1\le i\le k$，$b$ 中大于等于 $i$ 的数都恰有 $b_i$ 个，求子序列长度 $k$ 的最大值。

## 输入格式

输入的第一行有一个正整数 $n$，表示数列长度。

第二行有 $n$ 个正整数 $a_1,a_2,\ldots,a_n$ 表示这个序列。

## 输出格式

输出这个子序列的最大长度。

## 样例 #1

### 样例输入 #1

```
7
5 5 4 5 3 3 2
```

### 样例输出 #1

```
5
```

## 提示

【样例解释】

$5,5,5,3,3$ 中有 $5$ 个数 $\ge 1$，有 $5$ 个数 $\ge 2$，有 $5$ 个数 $\ge 3$，有 $3$ 个数 $\ge 4$，有 $3$ 个数 $\ge 5$，因此这个数列确实符合题意。

同样符合题意的还有 $3,3,2$ 等，但是这不是最长的。

【数据范围】

| 子任务编号 | $n\le$ |      特殊性质      |  分值  | 依赖子任务 |
| :--------: | :------: | :----------------: | :----: | ---------- |
|   $1$   |  $16$  |                    | $19$ | 无         |
|   $2$   |  $50$  |                    | $30$ | 1          |
|   $3$   | $200$ |                    | $34$ | 2          |
|   $4$   | $1000$ |     $a_i=i$     | $1$ | 无         |
|   $5$   | $1000$ | $a_i\ge a_{i+1}$ | $27$ | 无         |
|   $6$   | $1000$ |                    | $39$ | 3,4,5      |

对于全体数据，保证 $1\le a_i\le n\le 1000$，输入皆为整数。

**注意：本题略卡常，时间限制仅为标准程序的 $2$ 倍以上。**

本题想出核心之后其实并没怎么想过怎么优化做法，欢迎吊打 std。
