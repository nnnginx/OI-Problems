## 题目描述

FJ 把杂志上所有的文章摘抄了下来并把它变成了字符串 $S$。他想删除其中的子串 $T$，他将删去 $S$ 中第一次出现的子串 $T$，然后不断重复这一过程，直到 $S$ 中不存在子串 $T$。

注意：每次删除一个子串后，可能会出现一个新的子串 $T$。

请帮助 FJ 完成操作并输出最后的 $S$。

## 输入格式

输入的第一行包含字符串 $S$。

输入的第二行包含字符串 $T$。

## 输出格式

输出一行，包含最后的 $S$。

```input1
whatthemomooofun
moo
```

```output1
whatthefun
```

## 数据范围与提示

对于 $100\%$ 的数据，有 $1\le |T|\le |S|\le 10^6$，字符集为小写英语字母，且 $S$ 不会被删空。

## 题目来源

[USACO February 2015 Contest](http://www.usaco.org/index.php?page=feb15results) Silver T1