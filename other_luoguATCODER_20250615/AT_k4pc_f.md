# AT_k4pc_f タイトル未定(Untitled)

## 题目描述

カガミズ正在为他的儿子キュウリ君准备圣诞礼物。

然而，カガミズ心里有点担心。因为キュウリ君非常喜欢竞赛编程，他可能会受到比赛中那些奇怪题目的启发，提出想要一个数组或图作为礼物的要求。

为了避免到时候措手不及，カガミズ决定提前问问キュウリ君想要什么圣诞礼物。キュウリ君给出了一份特别的要求：

「我想要一个能自然定义的问题！」

## 输入格式

输入包括一行：
$ N $ $ X_1 $ $ K_1 $ $ D_1 $ : $ X_N $ $ K_N $ $ D_N $

## 输出格式

- 如果不论如何添加点也无法满足题目条件，则输出 `impossible`。
- 如果可以满足条件，但即便添加点数最小化，也超过 $ 10^5 $，则输出 `too many`。
- 如果可以通过添加不超过 $ 10^5 $ 个点来满足条件，输出以下格式的具体例子：

  $ M $ $ A_1 $ … $ A_M $

其中，$ M $ 为添加的点数，$ A_j $ 为所添加点的坐标。要求 $ M $ 最大值不得超过 $ 10^5 $，每个 $ A_j $ 必须在 $ 32 $ 位有符号整数的范围内。**输出要求没有多余的空行或空格。（16:36 更新）**

## 输入输出样例 #1

### 输入 #1

```
2
0 2 1
2 2 1
```

### 输出 #1

```
1
1
```

## 输入输出样例 #2

### 输入 #2

```
2
0 2 1
3 2 1
```

### 输出 #2

```
2
-1 2
```

## 输入输出样例 #3

### 输入 #3

```
1
1 1 1
```

### 输出 #3

```
impossible
```

## 输入输出样例 #4

### 输入 #4

```
1
1 114514 1
```

### 输出 #4

```
too many
```

## 输入输出样例 #5

### 输入 #5

```
1
1 1 0
```

### 输出 #5

```
0
```

## 说明/提示

### 任务描述

在一维空间中分布有 $ N $ 个点，第 $ i $ 个点 $ P_i $ 的坐标是 $ X_i $。

希望通过添加一些新点，使得这 $ N $ 个点符合以下条件，这些条件由两个长度为 $ N $ 的整数序列 $ K $ 和 $ D $ 给出：

- 条件：对于每一个 $ i = 1, \ldots, N $，点 $ P_i $ 的第 $ K_i $ 近的点与它的距离应该为 $ D_i $。两点间的距离为其坐标差的绝对值。

计算距离时，必须考虑原有的 $ N $ 个点和新添加的点。某个点可以是自身最近的点，此时距离为 $ 0 $。

判断能否通过添加点满足上述条件。如果可以，则进一步判断是否可将添加点数量限制在 $ 10^5 $ 以内，并给出一种符合条件的方案。

要求所有坐标 $ X_i $、$ D_i $ 以及新添加点的坐标都是整数，并且新增点的坐标要在 $ 32 $ 位有符号整数范围内。

请注意，原有的 $ N $ 个点与新添加的点坐标允许重合。

### 约束

所有输入数据满足以下条件：

- $ 1 \leq N \leq 10^3 $。
- $ -10^9 \leq X_i \leq 10^9 $。
- $ 1 \leq K_i \leq 10^9 $。
- $ 0 \leq D_i \leq 10^9 $。

题目还设置了部分分数，额外条件如下：

- $ N \leq 10 $。
- $ K_i = 2 $。

### 示例解说

1. 在保证添加点数不超过 $ 10^5 $ 的情况下，无需寻找加点数最少的方案。因此，输出结果如：`2 -1 1` 也是允许的。
2. 要特别注意，一点与自身的距离为 $ 0 $。
3. 例如，在坐标 $ 2 $ 处添加 $ 114,513 $ 个点可以满足条件，但因无法在 $ 10^5 $ 个点内满足条件，应输出 `too many`。
4. 请务必注意，不要在输出中添加多余的空行。（16:36 更新）

 **本翻译由 AI 自动生成**