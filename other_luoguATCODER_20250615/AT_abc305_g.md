# AT_abc305_g [ABC305G] Banned Substrings

## 题目描述

给定一个由 $M$ 个长度不超过 $6$ 的仅由字母 $\texttt a$ 和 $\texttt b$ 组成的非空字符串集合 $S=\{s_1, s_2, ..., s_M\}$。

求有多少个字符串 $T$ 满足以下条件：

- 长度为 $N$ 且仅由字母 $\texttt a$ 和 $\texttt b$ 组成。
- 对于任意 $s_i\in S$，$T$ 中不包含 $s_i$ 作为连续的子串。

由于答案可能很大，所以对 $998244353$ 取模。

## 输入格式

输入共 $M+1$ 行，第一行包括两个整数 $N$ 和 $M$，表示字符串长度和非空字符串集合大小。接下来 $M$ 行，每行一个字符串 $s_i$。

## 输出格式

输出仅包含一个整数，表示满足条件的字符串 $T$ 的个数对 $998244353$ 取模后的结果。

## 输入输出样例 #1

### 输入 #1

```
4 3
aab
bbab
abab
```

### 输出 #1

```
10
```

## 输入输出样例 #2

### 输入 #2

```
20 1
aa
```

### 输出 #2

```
17711
```

## 输入输出样例 #3

### 输入 #3

```
1000000007 28
bbabba
bbbbaa
aabbab
bbbaba
baaabb
babaab
bbaaba
aabaaa
aaaaaa
aabbaa
bbaaaa
bbaabb
bbabab
aababa
baaaba
ababab
abbaba
aabaab
ababaa
abbbba
baabaa
aabbbb
abbbab
baaaab
baabbb
ababbb
baabba
abaaaa
```

### 输出 #3

```
566756841
```

## 说明/提示

$1\leq N\leq 10^{18}$

$1\leq M\leq 126$

$N$ 和 $M$ 是整数。

$s_i$ 是由字母 $a$ 和 $b$ 组成的长度不超过 $6$ 的非空字符串。

$s_i \neq s_j$（$1\leq i<j\leq M$）。