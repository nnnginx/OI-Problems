## 题目描述
Given a complete undirected graph of $n$ vertices and $n$ strings $s_1, s_2, \cdots, s_n$, the weight of edge connecting vertices $i$ and $j$ is equal to the length of the longest common substring (LCS) between $s_i$ and $s_j$. Compute the maximum total weight of any spanning tree on this graph.

A substring of a string can be obtained by removing some (possibly zero) characters from the beginning and/or the end of that string. For example, ``maca``, ``aca`` and ``cau`` are all substrings of ``macau``, while ``acu`` is not.

## 输入格式
There is only one test case in each test file.

The first line of the input contains one integer $n$ ($1 \leq n \leq 2 \times 10^6$) indicating the number of vertices and strings.

For the following $n$ lines, the $i$-th line contains one string $s_i$ ($1 \le |s_i| \le 2 \times 10^6$) consisting only of lowercase English letters.

It's guaranteed that the sum of lengths of all strings will not exceed $2 \times 10^6$.

## 输出格式
Output one line containing one integer indicating the answer.

## 题目大意
**【题目描述】**

给定一个有 $n$ 个顶点的完全无向图和 $n$ 个字符串 $s_1, s_2, \cdots, s_n$，连接顶点 $i$ 和 $j$ 的边的权重等于字符串 $s_i$ 和 $s_j$ 的最长公共子串（LCS）的长度。计算此图上任意生成树的最大总权重。

一个字符串的子串可以通过从该字符串的开头和/或结尾删除一些（可能为零）字符来获得。例如，“maca”、“aca” 和“cau”都是“macau”的子串，而“acu”不是。

**【输入格式】**

每个测试文件中包含一个测试用例。

输入的第一行包含一个整数 $n$ ($1 \leq n \leq 2 \times 10^6$)，表示顶点和字符串的数量。

接下来的 $n$ 行，第 $i$ 行包含一个字符串 $s_i$ ($1 \le |s_i| \le 2 \times 10^6$)，由小写英文字母组成。

保证所有字符串的长度之和不超过 $2 \times 10^6$。

**【输出格式】**

输出一行，包含一个整数，表示答案。

翻译来自于：[ChatGPT](https://chatgpt.com/)

```input1
4
icpc
macau
regional
contest
```

```output1
4
```

```input2
3
ababa
babab
aba
```

```output2
7
```

