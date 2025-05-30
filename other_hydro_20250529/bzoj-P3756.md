## 题目描述

在神秘的东方有一棵奇葩的树，它有一个固定的根节点（编号为 $1$）。树的每条边上都是一个字符，字符为 $a,b,c$ 中的一个，你可以从树上的任意一个点出发，然后沿着远离根的边往下行走，在任意一个节点停止，将你经过的边的字符依次写下来，就能得到一个字符串，例如：

![](./3306/file/pic1.gif)

在这棵树中我们能够得到的字符串是：`c`,`cb`,`ca`,`a`,`b`,`a`。

现在 pty 得到了一棵树和一个字符串 $S$。如果 $S$ 的一个子串 $[l,r]$ 和树上某条路径所得到的字符串完全相同，则我们称这个子串和该路径匹配。现在 pty 想知道，$S$ 的所有子串和树上的所有路径的匹配总数是多少？

## 输入格式

第一行一个正整数 $n$，含义如题面所述。  
接下来 $n-1$ 行，每行一个整数 $fa$，一个字符 $c$，字符和整数之间用一个空格隔开。  
第 $i$ 行的 $fa$ 代表第 $i$ 号节点的父亲， $c$ 表示第 $i$ 号节点和 $fa$ 的连边的字符。  
最后一行为字符串 $S$。

## 输出格式

输出共一行，表示匹配总数。

```input1
5
1 c
2 b
1 a
2 a
cba
```

```output1
5
```

## 样例说明

单个字符匹配的对数为四对，两个字符匹配的对数为一对：`cb`。

## 数据规模与约定

对于 $100\%$ 的数据，$n \le 8 \times 10^5$，树的最大深度 $\le 8 \times 10^5$。

此题存在版权，故原 BZOJ 不再支持提交，保留在此只供大家参考题面！ 望见谅！

