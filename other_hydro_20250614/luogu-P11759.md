## 题目描述
化学家 Dubravka 在她的实验室研究 DNA 分子。每个 DNA 分子由一系列字符表示，其中每个单独的字符都来自集合 $\{ \texttt{A,C,G,T} \}$。比如，$\texttt{A}$，$\texttt{ATG}$ 和 $\texttt{GTA}$ 是代表不同 DNA 分子的字符串。

Dubravka 可以在 DNA 分子的任何部分进行以下变化：

- $\texttt{A} \leftrightarrow \texttt{TC}$，也就是说，$\texttt{A}$ 和 $\texttt{TC}$ 是可以互相转化的。
- $\texttt{C} \leftrightarrow \texttt{AG}$。
- $\texttt{G} \leftrightarrow \texttt{CT}$。
- $\texttt{T} \leftrightarrow \texttt{GA}$。

Dubravka 经常通过连续应用这些变化来使得一个分子变为另一个分子。例如：

$$\texttt{AA} \rightarrow \texttt{TCA} \rightarrow \texttt{TAGA} \rightarrow \texttt{TAT}$$

Dubravka 目前的实验室里有 $N$ 个分子。编写一个程序，确定每对给定分子是否有可能通过应用这些变化从第一个分子获得第二个分子。

## 输入格式
第一行是自然数 $N (2\le N\le 100)$，即分子数。分子从 $1$ 到 $N$ 编号。

在接下来的 $N$ 行中，每行给出一个字符串，其中每个字符都是大写字母 $\texttt{A},\texttt{C},\texttt{G},\texttt{T}$ 中的一个。每个字符串由最少 $1$ 个字符和最多 $50000$ 个字符组成。

## 输出格式
输出 $N$ 行，在每一行中，打印一个恰好包含 $N$ 个字符的字符串。如果可以从分子 $i$ 获得分子 $j$，则第 $i$ 行中的第 $j$ 个符号应输出 $1$，否则输出 $0$。

```input1
4
A
C
G
T
```

```output1
1000
0100
0010
0001
```

```input2
 4
 AA
 TAT
 C
 CGTAC
```

```output2
1100
1100
0011
0011
```

```input3
4
AAA
CCC
TATA
CACA
```

```output3
1111
1111
1111
1111

```

## 提示
以下每点都描述了一个值为 $10$ 分的测试数据：

- $N\le 5$，每个字符串不超过 $4$ 个字符。
- 每个分子恰好包含 $2$ 个字符。
- 每个分子恰好包含 $3$ 个字符。
- 每个分子恰好包含 $4$ 个字符。
- 每个分子恰好包含 $5$ 个字符。
- 每个分子恰好包含 $6$ 个字符。

对于剩下 $40 \%$ 数据，没有特殊限制。

