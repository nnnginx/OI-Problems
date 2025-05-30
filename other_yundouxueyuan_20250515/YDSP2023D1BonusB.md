本道题目为本场比赛的 Bonus 题目，整体思维、难度、技巧以及知识面上与 S 组略有不同，欢迎各位强者来挑战~

**赛时公告（12:29）：本题的大样例和数据更新。**

# Description

有 $n$ 个集合 $S_1,S_2,\cdots,S_n$，初始全为空，需要  支持三种操作：

- $1 \space l \space r \space x$：将 $x$ 插入 $S_l,\cdots,S_r$。
- $2 \space l \space r \space x$：将 $x$ 从 $S_l,\cdots,S_r$ 删除。
- $3 \space u \space v$：询问 $S_u$ 是否为 $S_v$ 的子集。

**请留意数据范围。**

# Format

## Input

第一行两个正整数 $n,m$，表示集合个数和操作个数。

接下来 $m$ 行，每行为以下三种形式之一：

- $1 \space l \space r \space x$
- $2 \space l \space r \space x$
- $3 \space u \space v$

分别表示一种操作。

## Output

对于每个 $3$ 操作，输出一行 `YES` 或 `NO` 以回答询问。

# Samples

```input1
5 10
1 1 5 1
1 2 4 2
3 1 2
3 2 2
3 2 3
1 3 3 3
3 1 3
2 2 4 2
1 5 5 5
3 5 3
```

```output1
YES
YES
YES
YES
NO
```

|         最后一次修改操作         |  $S_1$  |   $S_2$   |    $S_3$    |   $S_4$   |   $S_5$   |
| :------------------------------: | :-------: | :---------: | :-----------: | :---------: | :---------: |
| $1 \space 1 \space 5 \space 1$ | $\{1\}$ |  $\{1\}$  |   $\{1\}$   |  $\{1\}$  |  $\{1\}$  |
| $1 \space 2 \space 4 \space 2$ | $\{1\}$ | $\{1,2\}$ |  $\{1,2\}$  | $\{1,2\}$ |  $\{1\}$  |
| $1 \space 3 \space 3 \space 3$ | $\{1\}$ | $\{1,2\}$ | $\{1,2,3\}$ | $\{1,2\}$ |  $\{1\}$  |
| $2 \space 2 \space 4 \space 2$ | $\{1\}$ |  $\{1\}$  |  $\{1,3\}$  |  $\{1\}$  |  $\{1\}$  |
| $1 \space 1 \space 5 \space 1$ | $\{1\}$ |  $\{1\}$  |  $\{1,3\}$  |  $\{1\}$  | $\{1,5\}$ |

以下的全部样例请参考下发文件：

[戳这里下载下发文件](./5261/file/ex_ds.zip)

```input2
见下发文件中的 ex_ds2.in
```

```output2
见下发文件中的 ex_ds2.ans
```

此样例符合子任务 $2$ 的限制。

```input3
见下发文件中的 ex_ds3.in
```

```output3
见下发文件中的 ex_ds3.ans
```

此样例符合子任务 $3$ 的限制。

```input4
见下发文件中的 ex_ds4.in
```

```output4
见下发文件中的 ex_ds4.ans
```

此样例符合子任务 $4$ 的限制。

```input5
见下发文件中的 ex_ds5.in
```

```output5
见下发文件中的 ex_ds5.ans
```

此样例符合子任务 $5$ 的限制。

```input6
见下发文件中的 ex_ds6.in
```

```output6
见下发文件中的 ex_ds6.ans
```

此样例符合子任务 $6$ 的限制。

```input7
见下发文件中的 ex_ds7.in
```

```output7
见下发文件中的 ex_ds7.ans
```

此样例符合子任务 $7$ 的限制。

# Limitation

对于所有数据，有：

- $1 \le n,m \le 10^5$
- $1 \le x \le 10^5$
- $1 \le l \le r \le 10^5$
- $1 \le u,v \le 10^5$
- 对于 $1$ 操作，保证操作之前这些集合中均不包含 $x$。
- 对于 $2$ 操作，保证在这次操作之前有一个对应的 $1 \space l \space r \space x$ 操作且这个操作插入的 $x$ 没被删除。
- **对于 $3$ 操作，令 $LIM=|S_v|-|S_u|$，保证 $0 \le LIM \le 2$，其中 $|S_u|,|S_v|$ 分别表示集合 $u,v$ 的大小。**

| 子任务 |                     特殊性质                     |  分值  |
| :----: | :----------------------------------------------: | :----: |
| $1$ |                 答案均为 `NO`                 | $1$ |
| $2$ |                 $n,m \le 2000$                 | $5$ |
| $3$ |                   $x \le 10$                   | $12$ |
| $4$ | 所有$1$ 操作的 $x$ 互不相同，没有 $2$ 操作 | $21$ |
| $5$ |                    $LIM=0$                    | $12$ |
| $6$ |                  $LIM \le 1$                  | $23$ |
| $7$ |                        无                        | $26$ |

> Fun Fact: subtask $1$ 本来设置的是 $0.45$ 分，但因为 OJ 显示不了小数，就改成 $1$ 了。
