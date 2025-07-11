# AT_agc057_f [AGC057F] Reflection

## 题目描述

在数轴上有三个点 $A, B, C$，坐标分别是 $a, b, c$，满足 $a \le b \le c$。每次可以进行以下两个操作中的一种：

- 将点 $A$ 关于点 $B$ 对称；
- 将点 $C$ 关于点 $B$ 对称。

操作可以无限进行，每做完一次操作后，将三个点按照坐标从小到大的顺序重新标注 $A, B, C$。

求操作过程中，产生不同三元组 $(a, b, c)$ 的个数模 $998244353$ 的结果。

## 输入格式

**本题包含多组测试数据**。

第一行一个正整数 $T$ 表示数据组数。

对于每组数据，包含一行三个整数 $a, b, c$，满足 $a \le b \le c$。

## 输出格式

对于每组数据，输出一行一个整数，表示答案。

## 输入输出样例 #1

### 输入 #1

```
6
1 3 5
-2 -2 5
0 1 3
31 41 59
-123456789 0 987654321
-1000000000000000000 0 1000000000000000000
```

### 输出 #1

```
5
2
9
70
182333351
5
```

## 说明/提示

$1 \le T \le 10^5,\ -10^{18} \le a \le b \le c \le 10^{18}$。