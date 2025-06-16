## 题目描述
设有两个二维向量 $\overrightarrow{A}(X_A, Y_A), \overrightarrow{B}(X_B, Y_B)$。给定 $L$，求 $(X_A, Y_A), (X_B, Y_B)$ 有多少种不同的取值，使得：

1. $X_A, Y_A, X_B, Y_B$ 均为正整数；
2. $\overrightarrow{A} \cdot \overrightarrow{B} \leq L$，其中 $\overrightarrow{A} \cdot \overrightarrow{B}$ 表示 $\overrightarrow{A}, \overrightarrow{B}$ 的内积，即 $X_A \cdot X_B + Y_A \cdot Y_B$。

## 输入格式
输入的第一行包含一个正整数 $L$，表示题目描述中的限制条件。

## 输出格式
输出一行包含一个整数表示答案。

```input1
2
```

```output1
1
```

```input2
3
```

```output2
5
```

## 提示
### 评测用例规模与约定

- 对于 $40\%$ 的评测用例，$L \leq 50$；
- 对于 $80\%$ 的评测用例，$L \leq 5000$；
- 对于所有评测用例，$1 \leq L \leq 2^{20}$。

