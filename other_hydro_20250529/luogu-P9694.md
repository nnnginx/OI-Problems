## 题目描述
Given $n$ strings $w_1, w_2, \cdots, w_n$, please select $k$ strings among them, so that the lexicographic order of string $v$ is minimized, and output the optimal string $v$. String $v$ satisfies the following constraint: $v$ is the longest common prefix of two selected strings with different indices. Also, $v$ is the lexicographically largest string among all strings satisfying the constraint.

More formally, let $\mathbb{S}$ be a set of size $k$, where all the elements in the set are integers between $1$ and $n$ (both inclusive) and there are no duplicated elements. Let $\text{lcp}(w_i, w_j)$ be the longest common prefix of string $w_i$ and $w_j$, please find a set $\mathbb{S}$ to minimize the lexicographic order of the following string $v$ and output the optimal string $v$.

$$
v = \max\limits_{i \in \mathbb{S}, j \in \mathbb{S}, i \ne j} \text{lcp}(w_i, w_j)
$$

In the above expression, $\max$ is calculated by comparing the lexicographic order of strings.

Recall that:
- String $p$ is a prefix of string $s$, if we can append some number of characters (including zero characters) at the end of $p$ so that it changes to $s$. Specifically, empty string is a prefix of any string.
- The longest common prefix of string $s$ and string $t$ is the longest string $p$ such that $p$ is a prefix of both $s$ and $t$. For example, the longest common prefix of ``abcde`` and ``abcef`` is ``abc``, while the longest common prefix of ``abcde`` and ``bcdef`` is an empty string.
- String $s$ is lexicographically smaller than string $t$ ($s \ne t$), if
  - $s$ is a prefix of $t$, or
  - $s_{|p| + 1} < t_{|p| + 1}$, where $p$ is the longest common prefix of $s$ and $t$, $|p|$ is the length of $p$, $s_i$ is the $i$-th character of string $s$, and $t_i$ is the $i$-th character of string $t$.
- Specifically, empty string is the string with the smallest lexicographic order.

## 输入格式
There are multiple test cases. The first line of the input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $k$ ($2\leq n\leq 10^6$, $2\leq k\leq n$) indicating the total number of strings and the number of strings to be selected.

For the following $n$ lines, the $i$-th line contains a string $w_i$ ($1\leq |w_i|\leq 10^6$) consisting of lower-cased English letters.

It's guaranteed that the total length of all strings of all test cases will not exceed $10^6$.

## 输出格式
For each test case output one line containing one string indicating the answer. Specifically, if the answer is an empty string, print $\texttt{EMPTY}$.

## 题目大意
**【题目描述】**

给定 $n$ 个字符串 $w_1, w_2, \cdots, w_n$，请选出恰好 $k$ 个字符串，最小化字符串 $v$ 的字典序，并输出这个最优的字符串 $v$。其中 $v$ 满足以下条件：$v$ 是被选出的字符串中，某两个编号不同的字符串的最长公共前缀。而且，$v$ 是所有满足条件的字符串中，字典序最大的字符串。

更正式地，令 $\mathbb{S}$ 表示一个大小为 $k$ 的集合，集合中的元素均为从 $1$ 到 $n$ 的整数（含两端），且没有重复的元素。令 $\text{lcp}(w_i, w_j)$ 表示字符串 $w_i$ 和 $w_j$ 的最长公共前缀，您需要找到一个集合 $\mathbb{S}$ 以最小化下述字符串 $v$ 的字典序，并输出这个最优的字符串 $v$。

$$
v = \max\limits_{i \in \mathbb{S}, j \in \mathbb{S}, i \ne j} \text{lcp}(w_i, w_j)
$$

上式中的 $\max$ 通过字典序比较两个字符串。

请回忆：
- 称字符串 $p$ 是字符串 $s$ 的前缀，若可以在 $p$ 的末尾添加若干个字符（包括零个字符）将它变成 $s$。特别地，空字符串是任意字符串的前缀。
- 字符串 $s$ 和 $t$ 的最长公共前缀是一个最长的字符串 $p$，满足 $p$ 既是 $s$ 的前缀，又是 $t$ 的前缀。例如，``abcde`` 与``abcef`` 的最长公共前缀为 ``abc``，而 ``abcde`` 与 ``bcdef`` 的最长公共前缀为空字符串。
- 称字符串 $s$ 的字典序小于字符串 $t$（$s \ne t$），若
  - $s$ 是 $t$ 的前缀，或
  - $s_{|p| + 1} < t_{|p| + 1}$，其中 $p$ 为 $s$ 和 $t$ 的最长公共前缀，$|p|$ 为 $p$ 的长度，$s_i$ 表示字符串 $s$ 的第 $i$ 个字符，$t_i$ 表示字符串 $t$ 的第 $i$ 个字符。
- 特别地，空字符串是字典序最小的字符串。

**【输入格式】**

有多组测试数据。第一行输入一个整数 $T$ 表示测试数据组数。对于每组测试数据：

第一行输入两个整数 $n$ 和 $k$（$2\leq n\leq 10^6$，$2\leq k\leq n$），表示字符串的总数和需要选择的字符串的数量。

对于接下来 $n$ 行，第 $i$ 行输入一个由小写字母构成的字符串 $w_i$（$1\leq |w_i|\leq 10^6$）。

保证所有数据中字符串长度之和不超过 $10^6$。

**【输出格式】**

每组数据输出一行一个字符串表示答案。特别地，若答案为空字符串，输出 $\texttt{EMPTY}$。

```input1
2
5 3
gdcpc
gdcpcpcp
suasua
suas
sususua
3 3
a
b
c
```

```output1
gdcpc
EMPTY
```

