### 题目描述

**请注意题目不寻常的时空限制。**

一个仅含 $\texttt{( ) ?}$ 的字符串是好的当且仅当可以把每个 $\texttt?$ 替换为 $\texttt($ 或 $\texttt)$ 使得最终形成一个匹配的括号串。

给定正整数 $n$，有 $q$ 组询问，对于每组询问给定一个 $k$，你需要求出有多少个长度为 $2n$ 的恰包含 $k$ 个 $\texttt?$ 的好字符串。

答案可能很大，对 $10^9+3579$（一个质数）取模。

### 输入格式

第一行两个正整数 $n,q$。

后 $q$ 行，每行一个非负整数 $k$ 描述一组询问。

### 输出格式

$q$ 行，每行回答一组询问，答案对 $10^9+3579$ 取模。

### 样例输入

```plain
5 5
1
2
3
4
5
```

### 样例输出

```plain
420
1646
3468
4423
3598
```

### 测试点约束

**本题采用捆绑测试。**

数据范围：

| Subtask | 分值 | 特殊性质 | 时间限制 |
|:---:|:---:|:---:|:---:|
| 1 | 10 | $n\le 100$ | 2 s |
| 2 | 30 | $q=1$ | 2 s |
| 3 | 20 | $n\le 10^5$ | 2 s |
| 4 | 40 | 无特殊限制 | 10 s |

对于全部数据，$1\le q\le n\le 10^7$，$0\le k\le n$。输入文件较大，请选手注意 IO 效率。

