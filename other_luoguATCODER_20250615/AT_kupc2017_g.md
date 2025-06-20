# AT_kupc2017_g encode/decode 2017

## 题目描述

你将参与一个指定的游戏，其规则如下：

1. 给定一棵树 $T$，它有 $N = 100$ 个顶点和 $M = 99$ 条边，此外还给定一个整数 $X$。树 $T$ 的顶点从 $1$ 到 $N$ 依次编号，对于每条边，有顶点 $a_i$ 和顶点 $b_i$ 直接相连。
2. 你可以在树 $T$ 中添加若干条边，但需确保不形成重边或自环，最后得到一个图 $G$。假设你添加了 $A$ 条边。
3. 移除图 $G$ 中所有树 $T$ 原有的边，并对顶点重新编号，得到一个新的图 $G'$。新图 $G'$ 拥有 $N = 100$ 个顶点和 $A$ 条边，其顶点从 $1$ 到 $N$ 依次编号，每条边连接顶点 $c_i$ 和顶点 $d_i$。
4. 记忆中关于树 $T$、图 $G$ 以及整数 $X$ 的信息将被遗忘。
5. 观察到新图 $G'$ 时，你需要声明一个整数 $Y$。如果 $X = Y$，则游戏成功。

你的目标是，无论给定何种树 $T$ 和整数 $X$，始终能够使游戏成功。请编写一个程序，依据给定的树 $T$ 和整数 $X$，确定如何添加边；并在给定新生成的图 $G'$ 时，正确推算出整数 $Y$。

### 输入输出格式

该题目包括 encode（编码）和 decode（解码）两个独立阶段：

- **encode 阶段**：给定树 $T$ 和整数 $X$，决定如何添加边。
  
- **decode 阶段**：给定新图 $G'$，推算出整数 $Y$。

#### 输入格式 (encode 阶段)

在 encode 阶段，输入格式如下：

输入的第 1 行是字符串 `encode`，接下来依次给出：

> `encode` $N$ $M$ $a_1$ $b_1$ $a_2$ $b_2$ $\ldots$ $a_M$ $b_M$ $X$

#### 输出格式 (encode 阶段)

输出为 $A + 1$ 行：

- 第 1 行输出整数 $A$。
- 接下来 $A$ 行中，第 $i$ 行输出你在第 $i$ 次所添加边的两个顶点编号，用空格分隔。

有关输出的注意事项：

- 如果添加的边形成的图有重边或自环，decode 阶段将不会执行。
- 输出中边的端点编号必须在 $1$ 至 $N$ 之间，否则也视为无效。

#### 输入格式 (decode 阶段)

在 decode 阶段，输入格式如下：

输入的第 1 行是字符串 `decode`，后续输入格式为：

> `decode` $N$ $A$ $c_1$ $d_1$ $c_2$ $d_2$ $\ldots$ $c_A$ $d_A$

#### 输出格式 (decode 阶段)

输出一个整数 $Y$。只有当 $X = Y$ 时才算正确。

### 数据范围与提示

- $N = 100$
- $M = 99$
- $T$ 是一棵树
- $1 \leq a_i, b_i \leq N$ ($1 \leq i \leq M$)
- $0 \leq X \leq 10^{18}$
- $0 \leq A \leq \binom{N}{2} - M = 4851$
- $1 \leq c_i, d_i \leq N$ ($1 \leq i \leq A$)
- 除 $X$ 外，所有参数均为整数

### 评判方式

评判采取以下步骤：

1. 启动两个进程，一个用于 encode，另一个用于 decode。
2. 向 encode 进程传入 encode 阶段的输入，不提供 `EOF`。
3. 等待 encode 进程正确输出并结束运行。
4. 检查输出的边，若这些边形成的图含有重边或自环，或者边的端点编号不在 $1$ 至 $N$ 之间，视为错误。
5. 向 decode 进程提供 decode 阶段的输入，不提供 `EOF`。
6. 等待 decode 进程正确输出并结束运行。
7. 若 $X = Y$，则判断为正确答案，否则为错误。

此外，若输出格式不符合要求，也视为错误。 

### 示例输入输出

#### 示例输入1 (encode 阶段)

```
encode
100 99
49 74
50 84
78 91
12 14
9 62
54 77
47 88
29 55
52 53
3 53
53 63
33 95
9 57
44 48
3 13
3 73
1 49
62 63
48 53
55 94
50 60
89 95
57 64
75 96
7 48
41 99
44 79
21 94
13 50
42 82
1 16
22 88
19 34
63 87
1 36
14 58
18 56
33 82
12 37
55 84
87 96
12 55
4 76
64 68
38 52
40 50
38 59
47 75
17 32
18 83
20 63
76 92
54 71
34 59
16 89
39 94
2 98
11 85
24 60
28 76
46 70
19 23
41 46
36 40
68 93
15 37
2 68
82 90
4 26
45 90
28 59
43 94
10 44
16 54
65 97
41 51
10 27
96 97
10 86
52 91
5 44
18 28
32 99
67 84
67 100
46 80
55 72
18 80
69 71
6 43
25 71
30 96
8 57
11 88
80 81
19 61
30 35
8 31
42 66
382174891210833608
```

#### 示例输出1 (encode 阶段)

```
2
1 2
2 4
```

#### 示例输入1 (decode 阶段)

```
decode
100 2
49 33
35 49
```

注意，新图 $G'$ 的顶点编号可能与原始树 $T$ 中的编号不同。

#### 示例输出1 (decode 阶段)

```
382174891210833608
```

 **本翻译由 AI 自动生成**

## 输入格式

无

## 输出格式

无