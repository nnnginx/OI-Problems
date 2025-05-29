## 题目描述
小 M 决定开始写日记，但她不愿意花费太多时间构思日记的内容。为此，她找来了一个长度为 $n$ 的字符串 $S$，决定任取 $S$ 的一个前缀 $P$，再任取 $S$ 的一个后缀 $Q$，将 $P$ 和 $Q$ 顺次连接起来得到的字符串 $P+Q$ 作为日记的内容。这里，空串也认为是 $S$ 的前缀和后缀，因此 $P$ 和 $Q$ 各有 $n+1$ 种取法。

当然了，这样形成的很多字符串是无意义的。具体而言，小 M 认为一个已知的长度为 $m$ 的字符串 $T$ 为重要信息，所有包含该重要信息作为子串的字符串都是有意义的，反之则是无意义的。

请你求出，小 M 一共能写出多少种本质不同的有意义的字符串。本质不同就是说，对于某个有意义的字符串 $A$ ，即使它可以被若干种取前缀和后缀的方式得到，也只应被计入一次。

## 输入格式
输入共两行。

第一行一个字符串 $S$。

第二行一个字符串 $T$。

## 输出格式
一行一个整数，所求答案。

```input1
aab
ab
```

```output1
7
```

```input2
mikageandspica
spica
```

```output2
140
```

```input3
见选手目录下的 diary/diary3.in 与 diary/diary3.ans。
```

```output3
见选手目录下的 diary/diary3.in 与 diary/diary3.ans。
```

```input4
见选手目录下的 diary/diary4.in 与 diary/diary4.ans。
```

```output4
见选手目录下的 diary/diary4.in 与 diary/diary4.ans。
```

```input5
见选手目录下的 diary/diary5.in 与 diary/diary5.ans。
```

```output5
见选手目录下的 diary/diary5.in 与 diary/diary5.ans。
```

## 提示
### 样例 1 解释

对于第一组样例，所有能够形成的有意义字符串分别为  `ab`，`aab`，`aaab`，`aaaab`，`aabaab`，`aabab`，`aabb`，一共 $7$ 种。

### 子任务

对于所有测试数据，保证 $1 \leq |S| \leq 5 \times 10^6$，$1 \leq |T| \leq 2|S|$，输入的字符串 $S$ 和 $T$ 仅包含小写英文字母。其中 $|S|,|T|$ 分别表示串 $S$ 和 $T$ 的长度。

![](https://cdn.luogu.com.cn/upload/image_hosting/j2ymssdo.png)

- 2023.8.21 添加一组 hack 数据。

