## 背景

本来这道题叫做地毯。然而一位张姓男子不同意，就改名成前缀了。

## 题面

给定整数 $n$ 和一个长度为 $n$ 的字符串 $s$ ，并定义数组 $a_i$ 为 $s$ 中前 $i$ 个字符中 `A` 的个数，定义数组 $b_i$ 为 $s$ 中前 $i$ 个字符中 `B` 的个数。

保证 $\forall s_i\in \{A,B\}$ 。

定义长度为 $n$ 的序列 $r_i$ ，满足

$$
r_i=\begin{cases}
0 & a_i=b_i\\
1 & a_i>b_i\\
-1 & a_i<b_i
\end{cases}
$$

进行 $n-1$ 次操作，其中第 $i$ 次操作交换 $s_i$ 和 $s_{i+1}$ 。**操作有后效性**。交换后， $a_i,b_i,r_i$ 可能会发生变化。

记录初始的 $r$ 序列和每次操作后的 $r$ 序列，问最终记录下了多少种不同的 $r$ 序列。

定义两个长度相同的数组不同，当且仅当这两个数组中至少有一对处于对应位置上的数不相等。

## 输入格式

第一行一个整数 $n$ 。

第二行一个长度为 $n$ 的字符串 $s$ 。

## 输出格式

第一行一个整数，表示答案。

## 样例

```input1
4
AABB
```

```output1
3
```

```input2
4
AAAA
```

```output2
1
```

```input3
10
BBBAAABBAA
```

```output3
5
```

```input4
172
AABAAAAAABBABAABBBBAABBAAABBABBABABABBAAABAAABAABAABBBBABBBABBABBBBBBBBAAABAAABAAABABBBAABAAAABABBABBABBBBBABAABAABBBABABBAAAABAABABBBABAAAABBBBABBBABBBABAABBBAAAABAAABAAAB
```

```output4
24
```

## 数据范围

对于 $20\%$ 的数据，保证 $1\le n\le 3\times 10^3$ 。

对于所有数据，保证 $1\le n\le 10^6$ 。

