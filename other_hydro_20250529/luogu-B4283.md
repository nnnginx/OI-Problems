## 题目描述
给定一个正整数 $N$，然后将 $N$ 分解成 $3$ 个正整数之和，计算出共有多少种符合要求的分解方法。要求：
1. 分解的 $3$ 个正整数各不相同；
2. 分解的三个正整数中**各个数位**都不含数字 $3$ 和 $7$。

例如：$N$ 为 $8$，可分解为 $(1, 1, 6)$、$(1, 2, 5)$、$(1, 3, 4)$、$(2, 2, 4)$、$(2, 3, 3)$，其中满足要求的分解方法有 $1$ 种，为 $(1, 2, 5)$。

## 输入格式
输入一个正整数 $N$（$5 < N < 501$），表示要分解的正整数。

## 输出格式
输出一个整数，表示共有多少种符合要求的分解方法。

```input1
8
```

```output1
1
```

