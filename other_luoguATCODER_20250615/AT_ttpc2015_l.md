# AT_ttpc2015_l グラフ色ぬり

## 题目描述

# 图的着色


[problemUrl]: https://atcoder.jp/contests/ttpc2015/tasks/ttpc2015_l

给定一个由 $ N $ 个顶点和 $ A+B $ 条边组成的简单有向图 $ G $。每个顶点都被标记为 $ 1,\ 2,\ …,\ N $。

这个图中有 $ A $ 条红色边和 $ B $ 条蓝色边。

我们将删除所有蓝色边得到的图称为 $ G' $。

请找出满足以下条件的图 $ G'' $ 中边数的最大值：

- $ G'' $ 是从 $ G $ 中删除 $ 0 $ 条或更多蓝色边后得到的图。
- 当将顶点 $ 1 $ 作为起点，顶点 $ N $ 作为终点时，$ G' $ 和 $ G'' $ 的最大流的值相等。其中所有边的容量均为 $ 1 $。

有关最大流的信息，请参阅[这里](https://ja.wikipedia.org/wiki/%E6%9C%80%E5%A4%A7%E3%83%95%E3%83%AD%E3%83%BC%E5%95%8F%E9%A1%8C)。

## 输入格式

输入以以下格式从标准输入中给出。

> $ N $ $ A $ $ B $ $ X_1 $ $ Y_1 $ $ X_2 $ $ Y_2 $ : $ X_{A+B} $ $ Y_{A+B} $

- 第一行包含三个整数，以空格分隔，分别为 $ N(2\ \leq\ N\ \leq\ 100) $、$ A(1\ \leq\ A\ \leq\ 200) $ 和 $ B(1\ \leq\ B\ \leq\ 200) $。
- 接下来的 $ A+B $ 行给出了图的边信息。其中第 $ i $ 行包含两个整数 $ X_i(1\ \leq\ X_i\ \leq\ N) $ 和 $ Y_i(1\ \leq\ Y_i\ \leq\ N) $，表示存在边 $ (X_i,\ Y_i) $。
- 边 $ (X_1,\ Y_1),\ (X_2,\ Y_2),\ …,\ (X_A,\ Y_A) $ 为红色边，边 $ (X_{A+1},\ Y_{A+1}),\ (X_{A+2},\ Y_{A+2}),\ ...,\ (X_{A+B},\ Y_{A+B}) $ 为蓝色边。
- 不存在 $ X_i\ =\ Y_i $ 的 $ i $。并且，如果 $ i\ \neq\ j $，则 $ Y_i\ \neq\ Y_j $ 或 $ X_i\ \neq\ X_j $。

## 输出格式

输出 $ G'' $ 的边数的最大值。将结果输出到标准输出，并在末尾包含换行符。

## 样例 #1

### 样例输入 #1

```
4 2 2
1 2
2 4
1 3
3 4
```

### 样例输出 #1

```
3
```

## 样例 #2

### 样例输入 #2

```
4 2 2
1 2
3 4
1 3
2 4
```

### 样例输出 #2

```
2
```

## 样例 #3

### 样例输入 #3

```
5 3 4
1 2
2 3
3 5
1 4
2 4
3 4
5 4
```

### 样例输出 #3

```
7
```

## 样例 #4

### 样例输入 #4

```
5 1 3
1 5
2 3
3 4
4 2
```

### 样例输出 #4

```
4
```

## 样例 #5

### 样例输入 #5

```
5 3 4 
1 2
2 3
3 4
1 5
2 5
3 5
4 5
```

### 样例输出 #5

```
3
```

## 输入输出样例 #1

### 输入 #1

```
4 2 2
1 2
2 4
1 3
3 4
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
4 2 2
1 2
3 4
1 3
2 4
```

### 输出 #2

```
2
```

## 输入输出样例 #3

### 输入 #3

```
5 3 4
1 2
2 3
3 5
1 4
2 4
3 4
5 4
```

### 输出 #3

```
7
```

## 输入输出样例 #4

### 输入 #4

```
5 1 3
1 5
2 3
3 4
4 2
```

### 输出 #4

```
4
```

## 输入输出样例 #5

### 输入 #5

```
5 3 4 
1 2
2 3
3 4
1 5
2 5
3 5
4 5
```

### 输出 #5

```
3
```

## 说明/提示

### 样例解释 3

在这种情况下，可以添加所有蓝色边。

### 样例解释 4

在这种情况下，也可以添加所有蓝色边。

### 样例解释 5

在这种情况下，无法添加任何蓝色边。