## 题目描述

兔子们在玩两个串的游戏。给定两个字符串 $S$ 和 $T$，兔子们想知道 $T$ 在 $S$ 中出现了几次，分别在哪些位置出现。

注意：$T$ 中可能有 $\texttt?$ 字符，这个字符可以匹配任何字符。

## 输入格式

两行两个字符串，分别代表 $S$ 和 $T$。

## 输出格式

第一行一个正整数 $k$，表示 $T$ 在 $S$ 中出现了几次。

接下来 $k$ 行正整数，分别代表 $T$ 每次在 $S$ 中出现的开始位置。按照从小到大的顺序输出，$S$ 下标从 $0$ 开始。

## 样例输入

```plain
bbabaababaaaaabaaaaaaaabaaabbbabaaabbabaabbbbabbbbbbabbaabbbababababbbbbbaaabaaabbbbbaabbbaabbbbabab
a?aba?abba
```

## 样例输出

```plain
0
```

## 数据规模与约定

$S$ 长度不超过 $10^5$，$T$ 长度不会超过 $S$。$S$ 中只包含小写字母，$T$ 中只包含小写字母和 $\texttt?$。