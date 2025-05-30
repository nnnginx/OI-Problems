## 题目描述

你算出了结果后，LCR 发现游戏匹配的随机对手「神犇」并没有走最优决策，于是她赢得了比赛并解密了数据。

现在 LCR 要将数据发送到 LOJ。然而近期网络环境不稳定，为了数据的安全传输，LCR 要在其中加入随机校验数列。

LCR 的随机数列 ${X_n}$ 可以由四个参数 $A, B, C, X_0$ 描述：

$$X_{n + 1} = ((A X_n + B) \bmod C) + 1\ (n \in \mathbb{N})$$

传输完成后，要检测该数列的随机性以验证传输是否出现问题。于是 LCR 随机选取了序列中下标位于 $[L_1, R_1]$ 的某个元素 $X_i$，以及下标位于 $[L_2, R_2]$ 的某个元素 $X_j$，请你帮忙计算 $\left\lceil \frac{X_i}{X_j} + \frac{X_j}{X_i} \right\rceil$ 的期望值。

为了避免精度误差，你只需要给出期望值乘以 $(R_1 - L_1 + 1)(R_2 - L_2 + 1)$ 的值对 $10^9 + 7$ （一个质数）取模的值即可。

## 输入格式

共一行，包含八个正整数 $A, B, C, X_0, L_1, R_1, L_2$ 和 $R_2$，相邻两个数字之间恰好有一个空格。

## 输出格式

共一行，包含一个数字，表示答案。

```input1
1 3 7 1 2 3 4 5
```

```output1
13
```

```input2
3 5 10 1 2 3 1 2
```

```output2
12
```

## 数据范围与提示

对于所有数据，$1 \leq A, B, C, X_0 \leq 10^6, 1 \leq L_1 \leq R_1 \leq 10^{18}, 1 \leq L_2 \leq R_2 \leq 10^{18}$。

|Subtask #|分值|$A,B,C,X_0$ 的限制|$R_1, R_2$ 的限制|
|:-:|:-:|:-:|:-:|
|1|$10$|$A, B, C, X_0 \leq 10^6$|$R_1,R_2 \leq 10^3$|
|2|$20$|$A, B, C, X_0 \leq 10^5$|$R_1,R_2 \leq 10^5$|
|3|$30$|$A, B, C, X_0 \leq 10^5$|$R_1,R_2 \leq 10^{18}$|
|4|$40$|$A, B, C, X_0 \leq 10^6$|$R_1,R_2 \leq 10^{18}$|

