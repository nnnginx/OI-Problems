## 题目描述

定义一个串 $s$ 能匹配 $S$ 当且仅当 $s$ 能可超出头尾得覆盖 $S$。如下图。

![pic1](https://hydro.org.cn/d/bzoj/p/3499/file/pic1.jpg)

给定 $S$，问不同的 $s$ 的个数。
$S$ 的长度 $\leq 2 * 10^5$。

## 输入格式

The only line of the standard input contains a non-empty word that is not longer than $2 * 10^5$ letters. It consists of small letters of English alphabet.

## 输出格式

The first line of the standard output should contain the number of quasi-templates of word $v$. The second line should contain the shortest word being a quasi-template of word $v$. If there is more than one such shortest word, output the lexicographically smallest from the shortest quasi-templates.

## 样例输入

```
aaaabaabaaaba
```

## 样例输出
```
10
aabaa
```


## 样例说明

The word from the sample input has 10 quasi-templates: aaaabaabaaab, aaaabaabaaaba, aaabaaba, aaabaabaa, aaabaabaaa, aaabaabaaaba, aabaa, aabaabaa, aabaabaaa, and abaabaaa.

## 数据规模与约定

保证输入的串长 $\leq 2 * 10^5$