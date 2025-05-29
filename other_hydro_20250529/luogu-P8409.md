## 题目描述
给你一个 $R$ 行 $C$ 列的矩阵 $a$，$|a_{i,j}| \le 10^4$。请使用若干次下述操作（次数尽量少），使得矩阵中 $\sum_i \sum_j a_{i,j}$ 尽可能大。



| 操作 | 示例 |  |
| :---: | :---: | :---: |
| `rotR i k` 将第 $i$ 行的元素循环右移 $k$ 位 | $\left(\begin{array}{ccc}1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \\ 10 & 11 & 12\end{array}\right)$ | $\xrightarrow{\operatorname{rotR} 3\ 1}\left(\begin{array}{ccc}1 & 2 & 3 \\ 4 & 5 & 6 \\ 9 & 7 & 8 \\ 10 & 11 & 12\end{array}\right)$ |
| `rotS j k` 将第 $j$ 列的元素循环下移 $k$ 位 | $\left(\begin{array}{ccc}1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \\ 10 & 11 & 12\end{array}\right)$ | $\xrightarrow{\text { rotS } 3\ 2}\left(\begin{array}{ccc}1 & 2 & 9 \\ 4 & 5 & 12 \\ 7 & 8 & 3 \\ 10 & 11 & 6\end{array}\right)$ |
| `negR i` 将第 $i$ 行的元素全部乘以 -1 。 该操作当且仅当该行任何一个元素均未乘以 -1 时有效 | $\left(\begin{array}{ccc}1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \\ 10 & 11 & 12\end{array}\right)$ | $\xrightarrow{\text { negR } 2}\left(\begin{array}{ccc}1 & 2 & 3 \\ -4 & -5 & -6 \\ 7 & 8 & 9 \\ 10 & 11 & 12\end{array}\right)$ |
| `negS j` 将第 $j$ 列的元素全部乘以 -1。 该操作当且仅当该列任何一个元素均未乘以 -1 时有效 | $\left(\begin{array}{ccc}1 & 2 & 3 \\ 0 & 0 & 0 \\ 7 & 8 & 9 \\ 10 & 11 & 12\end{array}\right)$ | $\xrightarrow{\text { negS } 1}\left(\begin{array}{ccc}-1 & 2 & 3 \\ 0 & 0 & 0 \\ -7 & 8 & 9 \\ -10 & 11 & 12\end{array}\right)$ |

## 输入格式
第一行：$r,c$。
接下来 $r$ 行：矩阵 $a$。

## 输出格式
第一行包含两个整数，第一个整数为 $\sum_i \sum_j a_{i,j}$ 的最大值，第二个数为操作数量 $t$。
接下来 $t$ 行，每行包含一组操作。

```input1
3 4
1 -2 5 200
-8 0 -4 -10
11 4 0 100
```

```output1
345 2
rotS 2 1
negR 2
```

```input2
3 3
8 -2 7
1 0 -3
-4 -8 3
```

```output2
34 4
rotR 1 1
rotS 3 1
negR 2
negR 3
```

## 提示
$1 \le R,C \le 100$，$|A_{i,j}|s \le 10^4$

#### 评分标准
若你求了个错误的最大和，或是执行的操作中有无效的，该测试点不得分，否则：

若 $t \le 5 \cdot RC$，你将得到该点的所有分数；

若 $5\cdot RC<T<10^5$，你将得到该点 $50\%$ 的分数；

若 $t > 10^5$，你将得不到该点的任何分数。

本题分值按 COCI 原题设置，满分 $130$。

