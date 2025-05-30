## 题目描述

Fish 是一条生活在海里的鱼。有一天他很无聊，就到处去寻宝。他找到了位于海底深处的宫殿，但是一扇带有密码锁的大门却阻止了他的前进。

通过翻阅古籍，Fish 得知了这个密码的相关信息：

1. 该密码的长度为 $N$。
2. 密码仅含小写字母。
3. 以每一个字符为中心的最长回文串长度。
4. 以每两个相邻字符的间隙为中心的最长回文串长度。

很快 Fish 发现可能有无数种满足条件的密码。经过分析，他觉得这些密码中字典序最小的一个最有可能是答案，你能帮他找到这个密码么？

注意：对于两个串 $A$ 和 $B$，如果它们的前 $i$ 个字符都相同，而 $A$ 的第 $i+1$ 个字符比 $B$ 的第 $i+1$ 个字符小，那么认为是则称密码 $A$ 的字典序小于密码 $B$ 的字典序，例如字符串 `abc` 字典序小于字符串 `acb`。如果密码 $A$ 的字典序比其他所有满足条件的密码的字典序都小，则密码 $A$ 是这些密码中字典序最小的一个。

## 输入格式

输入由三行组成。第一行仅含一个整数 $N$，表示密码的长度。第二行包含 $N$ 个整数，表示以每个字符为中心的最长回文串长度。第三行包含 $N-1$ 个整数，表示每两个相邻字符的间隙为中心的最长回文串长度。

## 输出格式

输出仅一行。输出满足条件的最小字典序密码。古籍中的信息是一定正确的，故一定存在满足条件的密码。

```input1
3
1 1 1
0 0
```

```output1
abc
```

```input2
3
1 3 1
0 0
```

```output2
aba
```

```input3
3
1 3 1
2 2
```

```output3
aaa
```

## 数据范围

对于 $20\%$ 的数据，保证 $1 \leq n \leq 100$。

另有 $30\%$ 的数据，保证 $1 \leq n \leq 1000$。

对于所有数据，保证 $1 \leq n \leq 10^5$。