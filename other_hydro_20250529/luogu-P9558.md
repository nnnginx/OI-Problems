## 题目描述
Recall the definition of a trie:

- A trie of size $n$ is a rooted tree with $n$ vertices and $(n - 1)$ edges, where each edge is marked with a character.
- Each vertex in a trie represents a string. Let $s(x)$ be the string vertex $x$ represents.
- The root of the trie represents an empty string. Let vertex $u$ be the parent of vertex $v$, and let $c$ be the character marked on the edge connecting vertex $u$ and $v$, we have $s(v) = s(u) + c$. Here $+$ indicates string concatenation, not the normal addition operation.
- The string each vertex represents is distinct.

We now present you a rooted tree with $(n + 1)$ vertices. The vertices are numbered $0, 1, \cdots, n$ and vertex $0$ is the root. There are $m$ key vertices in the tree where vertex $k_i$ is the $i$-th key vertex. It's guaranteed that all leaves are key vertices.

Please mark a lower-cased English letter on each edge so that the rooted tree changes into a trie of size $(n + 1)$. Let's consider the sequence $A = \{s(k_1), s(k_2), \cdots, s(k_m)\}$ consisting of all strings represented by the key vertices. Let $B = \{w_1, w_2, \cdots, w_m\}$ be the string sequence formed by sorting all strings in sequence $A$ from smallest to largest in lexicographic order. Please find a way to mark the edges so that sequence $B$ is minimized.

We say a string $P = p_1p_2\cdots p_x$ of length $x$ is lexicographically smaller than a string $Q = q_1q_2\cdots q_y$ of length $y$, if

- $x < y$ and for all $1 \le i \le x$ we have $p_i = q_i$, or
- there exists an integer $1 \le t \le \min(x, y)$ such that for all $1 \le i < t$ we have $p_i = q_i$, and $p_t < q_t$.

We say a string sequence $F = \{f_1, f_2, \cdots, f_m\}$ of length $m$ is smaller than a string sequence $G = \{g_1, g_2, \cdots, g_m\}$ of length $m$, if there exists an integer $1 \le t \le m$ such that for all $1 \le i < t$ we have $f_i = g_i$, and $f_t$ is lexicographically smaller than $g_t$.

## 输入格式
There are multiple test cases. The first line of th input contains an integer $T$ indicating the number of test cases. For each test case:

The first line contains two integers $n$ and $m$ ($1 \le m \le n \le 2 \times 10^5$) indicating the number of vertices other than the root and the number of key vertices.

The second line contains $n$ integers $a_1, a_2, \cdots, a_n$ ($0 \le a_i < i$) where $a_i$ is the parent of vertex $i$. It's guaranteed that each vertex has at most $26$ children.

The third line contains $m$ integers $k_1, k_2, \cdots, k_m$ ($1 \le k_i \le n$) where $k_i$ is the $i$-th key vertex. It's guaranteed that all leaves are key vertices, and all key vertices are distinct.

It's guaranteed that the sum of $n$ of all test cases will not exceed $2 \times 10^5$.

## 输出格式
For each test case output one line containing one answer string $c_1c_2\cdots c_n$ consisting of lower-cased English letters, where $c_i$ is the letter marked on the edge between $a_i$ and $i$. If there are multiple answers strings so that sequence $B$ is minimized, output the answer string with the smallest lexicographic order.

## 题目大意
**【题目描述】**

请回忆字典树的定义：

- 一棵大小为 $n$ 的字典树是一棵有 $n$ 个节点和 $(n - 1)$ 条边的有根树，每一条边都标有一个字符。
- 字典树中的每个节点都代表一个字符串，令 $s(x)$ 表示节点 $x$ 代表的字符串。
- 字典树的根代表的是空字符串。设节点 $u$ 为节点 $v$ 的父节点，设 $c$ 表示节点 $u$ 和 $v$ 之间的边上标有的字符，则 $s(v) = s(u) + c$。这里的 $+$ 代表字符串连接，而不是普通的加法。
- 所有节点代表的字符串互不相同。

给定一棵有 $(n + 1)$ 个节点的有根树，节点编号为 $0, 1, \cdots, n$，其中节点 $0$ 是根节点。树上共有 $m$ 个关键节点，其中第 $i$ 个关键节点的编号为 $k_i$。保证所有叶子节点都是关键节点。

请为每一条边标上一个小写字母，使得这棵有根树变为一棵大小为 $(n + 1)$ 的字典树。考虑所有关键节点代表的字符串构成的序列 $A = \{s(k_1), s(k_2), \cdots, s(k_m)\}$，设 $B = \{w_1, w_2, \cdots, w_m\}$ 是由序列 $A$ 中所有字符串按字典序从小到大排序后得到的字符串序列，您需要找到一个标记字母的方案，使得序列 $B$ 最小。

称长度为 $x$ 的字符串 $P = p_1p_2\cdots p_x$ 的字典序小于长度为 $y$ 的字符串 $Q = q_1q_2\cdots q_y$，若

- $x < y$ 且对于所有 $1 \le i \le x$ 有 $p_i = q_i$，或者
- 存在一个整数 $1 \le t \le \min(x, y)$，对于所有 $1 \le i < t$ 有 $p_i = q_i$，且 $p_t < q_t$。

称长度为 $m$ 的字符串序列 $F = \{f_1, f_2, \cdots, f_m\}$ 小于长度为 $m$ 的字符串序列 $G = \{g_1, g_2, \cdots, g_m\}$，若存在一个整数 $1 \le t \le m$，对于所有 $1 \le i < t$ 有 $f_i = g_i$，且 $f_t$ 的字典序小于 $g_t$ 的字典序。

**【输入格式】**

有多组测试数据。第一行输入一个整数 $T$ 表示测试数据组数。对于每组测试数据：

第一行输入两个正整数 $n$ 和 $m$（$1 \le m \le n \le 2 \times 10^5$）表示除了根节点以外的节点数量和关键节点的数量。

第二行输入 $n$ 个整数 $a_1, a_2, \cdots, a_n$（$0 \le a_i < i$），其中 $a_i$ 代表节点 $i$ 的父节点。保证每个节点至多有 $26$ 个子节点。

第三行输入 $m$ 个整数 $k_1, k_2, \cdots, k_m$（$1 \le k_i \le n$），其中 $k_i$ 代表第 $i$ 个关键节点的编号。保证所有叶子节点都是关键节点，且没有重复的关键节点。

保证所有测试数据 $n$ 之和不超过 $2 \times 10^5$。

**【输出格式】**

每组数据输出一行一个由小写字母组成的答案字符串 $c_1c_2\cdots c_n$，其中 $c_i$ 表示节点 $a_i$ 到 $i$ 的边上标有的小写字母。若有多种答案字符串使得字符串序列 $B$ 最小，请输出字典序最小的答案字符串。

**【样例解释】**

第一组样例数据的答案如下图所示。

![](https://cdn.luogu.com.cn/upload/image_hosting/zvhqplsb.png)

其中，节点 $1$ 代表的字符串为 ``a``，节点 $4$ 代表的字符串为 ``aba``，节点 $3$ 代表的字符串为 ``aa``，节点 $5$ 代表的字符串为 ``abb``。因此 $B = \{$``a``, ``aa``, ``aba``, ``abb``$\}$。

```input1
2
5 4
0 1 1 2 2
1 4 3 5
1 1
0
1
```

```output1
abaab
a
```

## 提示
The answer of the first sample test case is shown as follows.

![](https://cdn.luogu.com.cn/upload/image_hosting/zvhqplsb.png)

The string represented by vertex $1$ is ``a``. The string represented by vertex $4$ is ``aba``. The string represented by vertex $3$ is ``aa``. The string represented by vertex $5$ is ``abb``. So $B = \{$``a``, ``aa``, ``aba``, ``abb``$\}$.

