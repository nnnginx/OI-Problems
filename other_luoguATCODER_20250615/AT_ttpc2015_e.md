# AT_ttpc2015_e マス目色ぬり

## 题目描述

### 题目大意
您将得到一个 $ N × N $ 的平方。 设  $ i(1\ \leq\ i\ \leq\ N) $  从顶部开始， $ j(1\ \leq\ j\ \leq\ N) $  从左边方块 $ (i,\ j) $

如果 $ i+j $ 是偶数，则每个单元格涂成红色，如果是奇数，则涂蓝色。

然后，对于 $K$ 美元的方块，如果它们被涂成红色，则将它们重新粉刷成蓝色，如果它们被涂成蓝色，则重新粉刷成红色。

之后，你选择几个方块。 但是，选定的方块必须是一个没有单个孔的矩形。

我想确保所选单元格中红色单元格的数量和蓝色单元格的数量之间的绝对差异尽可能大。 最多有多少个？

## 输入格式

输入由标准输入给出，格式如下：

> $ N $ $ K $ $ Y_1 $ X_1 $ $ Y_2 $ $ X_2 $ ： $ Y_K $ $ X_K $

- $ 1 $ 整数  $ N(1\ \leq\ N\ \leq\ 2000) $、$ K(1\ \leq\ K\ \leq\ 10) $ 在用空格分隔的行中给出。
- 之后，给出 $ K $ 行要重新着色的单元格的信息。 在 $ i $ 行中，整数 $ Y_i(1\ \leq\ Y_i\ \leq\ N) $、$ X_i(1\ \leq\ X_i\ \leq\ N) $  以空格分隔的形式给出，表示 $ （Y_i， X_i） $ 的颜色将被重新绘制。
- 如果 $ i\ \neq\ j $ 满足 $ Y_i\ \neq\ Y_j $ 或 $ X_i\ \neq\ X_j $。

## 输出格式

输出红色单元格数和蓝色单元格数之差的最大绝对值。 输出应为标准输出，末尾带有换行符。

## 输入输出样例 #1

### 输入 #1

```
3 1
1 1
```

### 输出 #1

```
2
```

## 输入输出样例 #2

### 输入 #2

```
3 4
1 2
2 1
2 3
3 2
```

### 输出 #2

```
9
```

## 输入输出样例 #3

### 输入 #3

```
3 4
1 1
1 3
3 1
3 3
```

### 输出 #3

```
7
```