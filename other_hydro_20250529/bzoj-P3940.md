## 题目描述

FJ 把杂志上所有的文章摘抄了下来并把它变成了字符串 $S$。他有一个包含 $n$ 个单词的列表，列表里的 $n$ 个单词记为 $t_1\sim t_N$。他希望从 $S$ 中删除这些单词。

FJ 每次在 $S$ 中找到最早出现的列表中的单词（最早出现指该单词的开始位置最小），然后从 $S$ 中删除这个单词。他重复这个操作直到 $S$ 中没有列表里的单词为止。注意删除一个单词后可能会导致 $S$ 中出现另一个列表中的单词。

FJ 注意到列表中的单词不会出现一个单词是另一个单词子串的情况，这意味着每个列表中的单词在 $S$ 中出现的开始位置是互不相同的。

请帮助 FJ 完成这些操作并输出最后的 $S$。

## 输入格式

第一行包含一个字符串 $S$。

第二行包含一个整数 $N$。

接下来 $N$ 行，每行包含一个字符串，第 $i$ 行的字符串是 $t_i$。

## 输出格式

输出一行，包含操作后的 $S$。

```input1
begintheescapexecutionatthebreakofdawn
2
escape
execution
```

```output1
beginthatthebreakofdawn
```

## 数据规模与约定

对于 $100\%$ 的数据，有 $1\le |S|,\sum|t_i|\le 10^5$， $1\le N\le 2000$，字符集为小写英语字母，保证 $S$ 不会被删空。

## 题目来源

[USACO February 2015 Contest](http://www.usaco.org/index.php?page=feb15results) Gold T2