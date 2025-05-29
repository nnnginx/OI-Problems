## 题目背景
原题译自 [POI 2024/2025 R1 Sprawiedliwy podział](https://sio2.mimuw.edu.pl/c/oi32-1/p/spr/)。

## 题目描述
Bajtyna 和 Bitek 需要分配他们拥有的 $n$ 件物品。对于每件物品，我们知道其对 Bajtyna 和 Bitek 的价值；这两个价值可以相同，也可以不同。我们希望将每件物品分配给其中一人，且没有人对另一人感到嫉妒，具体定义如下。

如果 Bitek 分到的所有物品的总价值严格小于 Bajtyna 分到的所有物品总价值减去其中任意一个（尤其是价值最小的一个），则 Bitek 会嫉妒 Bajtyna。例如，考虑四件物品，对 Bitek 的价值分别为 $4, 3, 4, 8$。如果将前两个物品分配给 Bitek，Bitek 会嫉妒 Bajtyna，因为 $4 + 3 < 8$。如果将最后一个物品分配给 Bitek，他不会嫉妒 Bajtyna，因为 $8 \geq 4 + 4$。

类似地，我们定义 Bajtyna 何时会嫉妒 Bitek，对于这种情况我们计算的是 Bajtyna 分到的所有物品的总价值。

请将所有物品分配给 Bajtyna 和 Bitek，使得没有人会嫉妒对方。

## 输入格式
输入的第一行包含一个整数 $n (1 \leq n \leq 5\cdot 10^5)$，表示物品的数量。第二行包含 $n$ 个整数 $a_{1}, a_{2}, \ldots, a_{n} (1 \leq a_{i} \leq 10^9)$，表示每件物品对 Bajtyna 的价值。第三行包含 $n$ 个整数 $b_{1}, b_{2}, \ldots, b_{n} (1 \leq b_{i} \leq 10^9)$，表示每件物品对 Bitek 的价值。

## 输出格式
在输出的第一行中，输出 $n$ 个用空格分隔的整数，描述满足条件的物品分配方案。第 $i$ 个数字应为 $0$，表示第 $i$ 件物品分配给 Bajtyna，或为 $1$，表示分配给 Bitek。可以假设总存在满足题目要求的分配方案。

```input1
4
10 5 9 6
4 6 8 4
```

```output1
1 0 0 1
```

```input2
见下发 spr1ocen.in
```

```output2
见下发 spr1ocen.out
```

```input3
见下发 spr2ocen.in
```

```output3
见下发 spr2ocen.out
```

```input4
见下发 spr3ocen.in
```

```output4
见下发 spr3ocen.out
```

## 提示
对于样例一，将第二和第三件物品分配给 Bajtyna，其他分配给 Bitek。Bajtyna 不会嫉妒 Bitek，因为 $5+9 \geq 10$ 和 $5+9 \geq 6$。Bitek 不会嫉妒 Bajtyna，因为 $4+4 \geq 6$ 和 $4+4 \geq 8$。

对于样例二，该样例满足 $n=6,a_i=7-i,b_i=i$。

对于样例三，该样例满足 $n=12, a_{i}=1, b_{i}=2$。

对于样例四，该样例满足 $n=5\cdot 10^5, a_{i}=b_{i}=10^9$。

| 子任务编号 | 特殊性质 | 分值 |
| :----------- | :----------- | :----------- |
| $1$ | $n \leq 10$ | $9$ |
| $2$ | $n \leq 20$ | $10$ |
| $3$ | $a_i=b_i$ | $40$ |
| $4$ | $n \leq 1000$ | $15$ |
| $5$ | 无特殊性质 | $26$ |

子任务 $0$ 为样例。

