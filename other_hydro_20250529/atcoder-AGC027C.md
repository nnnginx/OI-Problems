分数 : $900$ 分

## 问题陈述

给定一个由 $N$ 个顶点和 $M$ 条边组成的无向图。  
顶点编号从 $1$ 到 $N$，边编号从 $1$ 到 $M$。  
此外，每个顶点都有一个标签，`A` 或 `B`。顶点 $i$ 的标签为 $s_i$。  
边 $i$ 双向连接顶点 $a_i$ 和 $b_i$。

幽灵窃贼 Nusook 喜欢选择某个顶点作为起点，并沿着边行走零次或多次。  
今天，他将在如上所述的旅行后生成一个字符串，按访问顺序将访问过的顶点的标签放在一起，从起点开始。

例如，在一个图中，顶点 $1$ 的标签为 `A`，顶点 $2$ 的标签为 `B`，如果 Nusook 沿着路径 $1 \rightarrow 2 \rightarrow 1 \rightarrow 2 \rightarrow 2$ 行走，则生成的字符串为 `ABABB`。

确定 Nusook 是否能够生成由 `A` 和 `B` 组成的所有字符串。

## 约束条件

- $2 \leq N \leq 2 \times 10^{5}$
- $1 \leq M \leq 2 \times 10^{5}$
- $|s| = N$
- $s_i$ 是 `A` 或 `B`。
- $1 \leq a_i, b_i \leq N$
- 给定的图可能不是简单图或连通图。

## 输入

输入格式如下所示，从标准输入中给出：

> $N$ $M$  
>  
> $s$  
>  
> $a_1$ $b_1$  
>  
> $:$  
>  
> $a_{M}$ $b_{M}$

## 输出

如果 Nusook 能够生成由 `A` 和 `B` 组成的所有字符串，打印 `Yes`；否则，打印 `No`。

```input1
2 3
AB
1 1
1 2
2 2
```

```output1
Yes
```

- 因为 Nusook 可以以任何方式访问顶点 $1$ 和顶点 $2$，他可以生成所有由 `A` 和 `B` 组成的字符串。

![77e96cf8e213d606ddd8f3c3f8315d32.png](https://img.atcoder.jp/agc027/77e96cf8e213d606ddd8f3c3f8315d32.png)

```input2
4 3
ABAB
1 2
2 3
3 1
```

```output2
No
```

- 例如，Nusook 无法生成 `BB`。  
- 给定的图可能不连通。

![1ab1411cb9d6ee023d14ca4e77c4b584.png](https://img.atcoder.jp/agc027/1ab1411cb9d6ee023d14ca4e77c4b584.png)

```input3
13 23
ABAAAABBBBAAB
7 1
10 6
1 11
2 10
2 8
2 11
11 12
8 3
7 12
11 2
13 13
11 9
4 1
9 7
9 6
8 13
8 6
4 10
8 7
4 3
2 1
8 12
6 9
```

```output3
Yes
```

```input4
13 17
BBABBBAABABBA
7 1
7 9
11 12
3 9
11 9
2 1
11 5
12 11
10 8
1 11
1 8
7 7
9 10
8 8
8 12
6 2
13 11
```

```output4
No
```