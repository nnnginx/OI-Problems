## 题目描述
我们定义一种名为「行列式」的新运算：

对于四个整数 $a, b, c, d$，我们定义 $\begin{vmatrix} a & b \\ c & d \end{vmatrix}$ 为 $a, b, c, d$ 的行列式，其等于 $a \times d - b \times c$。

现在，给定 $a, b, c, d$，请你帮忙计算 $\begin{vmatrix} a & b \\ c & d \end{vmatrix}$ 的值是多少。

## 输入格式
输入共一行四个整数 $a, b, c, d$。

## 输出格式
输出共一行一个整数，代表 $\begin{vmatrix} a & b \\ c & d \end{vmatrix}$ 的值。

```input1
3 7 4 9
```

```output1
-1
```

## 提示
### 样例 1 说明

$\begin{vmatrix} 3 & 7 \\ 4 & 9 \end{vmatrix} = 3 \times 9 - 4 \times 7 = -1$。

### 数据规模与约定

对于 $100\%$ 的数据，保证 $-10 ^ 9 \leq a, b, c, d \leq 10 ^ 9$。

