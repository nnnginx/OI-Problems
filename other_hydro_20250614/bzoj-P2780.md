## 题目描述

Oimaster and sevenk love each other.

But recently,sevenk heard that a girl named ChuYuXun was dating with oimaster.As a woman's nature, sevenk felt angry and began to check oimaster's online talk with ChuYuXun.

Oimaster talked with ChuYuXun $n$ times, and each online talk actually is a string.Sevenk asks $q$ questions like this,   **"how many strings in oimaster's online talk contain this string as their substrings?"**

题意：给出 $n$ 个串 $a_i$，$q$ 次询问，每次给定一个串 $s_i$，问 $s_i$ 是多少个 $a_i$ 的子串。

## 输入格式

There are two integers $n,q$ in the first line, the number of strings ​and the number of questions.  
And $n$ lines follow, each of them is a string describing oimaster's online talk.   
And $q$ lines follow, each of them is a question.

## 输出格式

For each question, output the answer in one line.

```input1
3 3
abcabcabc
aaa
aafe
abc
a
ca
```

```output1
1
3
1
```

## 数据规模与约定

对于 $100\%$ 的数据，$1\leq n\leq10^4$，$1\leq q\leq 6\times 10^4$，$\sum |a_i|\leq 10^5$，$\sum |s_i| \leq 3.6\times 10^5$。