# AT_code_festival_2017_qualc_e Cubes

## 题目描述

我们用边长为 $1$ 的小立方体搭建了一个 $A \times B \times C$ 的长方体。接着，我们将这个长方体放置在 $xyz$ 空间中，使其满足以下条件：

- 对于所有的 $i, j, k$（$0 \leq i < A, 0 \leq j < B, 0 \leq k < C$），存在一块立方体，其对角线连接着点 $(i, j, k)$ 和 $(i+1, j+1, k+1)$，并且该块的所有边都平行于坐标轴。

我们将每个这样的立方体块称为块 $(i, j, k)$。

定义两块立方体 $(i_1, j_1, k_1)$ 和 $(i_2, j_2, k_2)$ 之间的距离为：$\max(|i_1 - i_2|, |j_1 - j_2|, |k_1 - k_2|)$。

现在，我们在从点 $(0, 0, 0)$ 到点 $(A, B, C)$ 的对角线上穿过一根很细的针线。请计算满足以下条件的立方体块 $(x, y, z)$ 的数量，并输出对 $10^9 + 7$ 取模的结果：

- 存在一个被针线穿过的（不算仅仅接触边界的情况）块 $(x', y', z')$，使得块 $(x, y, z)$ 与块 $(x', y', z')$ 的距离不大于 $D$。

## 输入格式

输入以如下格式给出：

> $A$ $B$ $C$ $D$

## 输出格式

输出满足条件的立方体块的数量，并对 $10^9 + 7$ 取模。

## 输入输出样例 #1

### 输入 #1

```
3 4 5 1
```

### 输出 #1

```
54
```

## 输入输出样例 #2

### 输入 #2

```
1 2 3 0
```

### 输出 #2

```
4
```

## 输入输出样例 #3

### 输入 #3

```
3 5 7 100
```

### 输出 #3

```
105
```

## 输入输出样例 #4

### 输入 #4

```
3 123456781 1000000000 100
```

### 输出 #4

```
444124403
```

## 输入输出样例 #5

### 输入 #5

```
1234 12345 1234567 5
```

### 输出 #5

```
150673016
```

## 输入输出样例 #6

### 输入 #6

```
999999997 999999999 1000000000 50000
```

### 输出 #6

```
8402143
```

## 说明/提示

- $1 \leq A < B < C \leq 10^9$
- $A, B, C$ 都两两互质
- $0 \leq D \leq 50,000$

### 样例说明

#### 样例 1

图中展示的是将长方体沿平行于 $xy$ 平面的方向分成 $5$ 层后的样子。其中第 $i$ 层包括 $i-1 \leq z \leq i$ 的块。黑色块表示被针线穿过且满足条件的块，黄色块是除这些外满足条件的块。所有黄黑两色的块总共为 $54$ 个。

#### 样例 2

被针线穿过的块有 $4$ 个，且仅这些块满足条件。

#### 样例 3

所有块都满足条件。

 **本翻译由 AI 自动生成**