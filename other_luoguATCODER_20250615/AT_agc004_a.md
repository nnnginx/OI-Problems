# AT_agc004_a [AGC004A] Divide a Cuboid

## 题目描述

用若干个 $ 1 \times 1 \times 1 $ 的小方块（立方体）组成一个 $ A \times B \times C $ 的大长方体，每个小方块可以涂成红色或蓝色，但要满足以下要求：

① 至少有 $1$ 个红色方块与 $1$ 个蓝色方块。

② 所有的红色方块必须组成一个长方体。

③ 所有的蓝色方块必须组成一个长方体。

求所有满足要求的染色方案中，红色方块数与蓝色方块数相差个数的最小值。

## 输入格式

一行 $3$ 个正整数，分别是 $ A, B, C $。

## 输出格式

一行 $1$ 个数，表示所求的答案。

## 输入输出样例 #1

### 输入 #1

```
3 3 3
```

### 输出 #1

```
9
```

## 输入输出样例 #2

### 输入 #2

```
2 2 4
```

### 输出 #2

```
0
```

## 输入输出样例 #3

### 输入 #3

```
5 3 5
```

### 输出 #3

```
15
```

## 说明/提示

$ 2 ≤ A, B, C ≤ 10^9 $

感谢@刷题永动机 提供的翻译