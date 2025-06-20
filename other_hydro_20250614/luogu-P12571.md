## 题目描述
This is an interactive problem.

A string is considered a palindrome if it reads the same from both sides. Formally, a string $s$ of length $n$ is considered a palindrome if $s_i = s_{n-i+1}$ for $1 \le i \le n$. For example, the strings ``gg``, ``ara``, ``abacaba``, and ``rotator`` are palindromes, while the strings ``array``, ``palindrome``, and ``uoi`` are not.

We call a string a **nearly palindrome** if its characters can be rearranged to form a palindrome. For example, the strings ``n``, ``ara``, ``arr``, and ``array`` are nearly palindromes, while the strings ``palindrome``, ``uoi``, and ``random`` are not.

A substring of a string is a string that can be obtained by deleting some (possibly zero) elements from its beginning and end.

Let $f(s)$ be the maximum length among the lengths of substrings of $s$ that are **not** nearly palindromes, or $0$ if there are no such substrings.

You are given a string $s$ of length $n$ consisting of lowercase Latin letters. You are also given $q$ queries of the form $l_i$, $r_i$. For each query, find the value of $f(s[l_i..r_i])$, where $s[l_i..r_i]$ denotes the substring consisting of characters $s_{l_i}, s_{l_{i} + 1}, \ldots, s_{r_i}$.

## 输入格式
The first line contains one integer $n$ ($1 \le n \le 2\cdot 10^5$) --- the length of the string.

The second line contains a string $s$ consisting of $n$ lowercase Latin letters.

The third line contains one integer $q$ ($1\le q \le 2\cdot 10^5$) --- the number of queries.

The fourth line contains two integers $l_1, r_1$ ($1 \leq l_1 \leq r_1 \leq n$) --- the parameters of the first query.

You will receive the parameters of the next queries from the jury program (see section Interaction Protocol).

### Interaction Protocol


The jury program will output two integers $l_i$, $r_i$ ($1\le l_i\le r_i\le n$) on separate lines for each query, starting from the second one.

The jury program will not output the parameters for the next query until it reads the response of your program to the previous query.

Make sure to call the $\texttt{flush}$ method after outputting each line. You can use:

- $\texttt{fflush(stdout)}$, $\texttt{cout <{}< endl}$, or $\texttt{cout.flush()}$ in $\tt{C++}$;
- $\texttt{System.out.flush()}$ in $\tt{Java}$;
- $\texttt{flush(output)}$ in $\tt{Pascal}$;
- $\texttt{sys.stdout.flush()}$ in $\tt{Python}$;
- consult the documentation for other programming languages.

## 输出格式
For each $i$-th query, output one integer --- the value of $f(s[l_i..r_i])$, in a separate line.

```input1
8
aabaaaba
3
3 7
1 8
4 4
```

```output1
4
6
0
```

## 提示
In the first example, you need to find the answers to three queries:

- $s[3..7] =\;$``baaab``, which has a substring ``aaab`` of length 4, which is not an **almost palindrome**;
- $s[1..8] =\;$``aabaaaba``, which has a substring ``aabaaa`` of length 6, which is not an **almost palindrome**;
- $s[4..4] =\;$``a``, all substrings of which are **almost palindromes**.

### Scoring

- ($6$ points): $q=1$, $l_1=1$, $r_1=n$, $n$ is even, $s$ has the form ``aabbaabbaa...``;
- ($9$ points): $q=1$, $l_1=1$, $r_1=n$, $n \le 200$;
- ($5$ points): $q=1$, $l_1=1$, $r_1=n$, $n \le 5000$;
- ($8$ points): $q=1$, $l_1=1$, $r_1=n$;
- ($10$ points): $s$ contains only letters $\tt{a}$ and $\tt{b}$;
- ($8$ points): $s_{l_i} \neq s_{r_i}$ for $1 \le i \le q$;
- ($7$ points): $s_i \neq s_{i+1}$ for $1 \le i < n$;
- ($10$ points): $s$ contains only letters $\tt{a}, \tt{b}, \tt{c}, \tt{d}, \tt{e}$, and $\tt{f}$;
- ($18$ points): $(r_i-l_i+1)$ is odd for $1\le i\le q$;
- ($19$ points): without additional constraints.

