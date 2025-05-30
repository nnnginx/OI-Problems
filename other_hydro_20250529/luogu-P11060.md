## 题目背景
原题链接：<https://oier.team/problems/X4A>。

## 题目描述
给定一个非负整数 $n$，判断 $n!$ 是否是 $n+1$ 的倍数，如果是则输出 `YES`，否则输出 `NO`。

其中 $n!$ 表示 $n$ 的阶乘，其值为所有小于等于 $n$ 的正整数的乘积。例如 $3! = 1 \times 2 \times 3 = 6$。并额外规定 $0! = 1$。

## 输入格式
仅一行，一个非负整数 $n$。

## 输出格式
仅一行一个字符串 `YES` 或 `NO`，表示 $n!$ 是否是 $n+1$ 的倍数。

```input1
0

```

```output1
YES

```

```input2
3

```

```output2
NO

```

```input3
6

```

```output3
NO

```

```input4
7

```

```output4
YES

```

```input5
15

```

```output5
YES

```

## 提示
**【样例解释 #1】**

$0! = 1$，而 $1$ 是 $1$ 的倍数，故输出 `YES`。

**【样例解释 #2】**

$3! = 1 \times 2 \times 3 = 6$，而 $6$ 不是 $4$ 的倍数，故输出 `NO`。

**【样例解释 #3】**

$6! = 1 \times 2 \times 3 \times 4 \times 5 \times 6 = 720$，而 $720$ 不是 $7$ 的倍数，故输出 `NO`。

**【样例解释 #4】**

$7! = 1 \times 2 \times 3 \times 4 \times 5 \times 6 \times 7= 5040$，而 $5040$ 是 $8$ 的倍数，故输出 `YES`。

**【样例解释 #5】**

$15! = 1 \times 2 \times 3 \times 4 \times 5 \times 6 \times 7 \times 8 \times 9 \times 10 \times 11 \times 12 \times 13 \times 14 \times 15 = 1{,}3076{,}7436{,}8000$，而 $1{,}3076{,}7436{,}8000$ 是 $16$ 的倍数，故输出 `YES`。

**【数据范围】**

本题共有 $20$ 个测试点，第 $i$ 个测试点的 $n$ 为 $i-1$。

对于 $100\%$ 的数据，$0 \le n \le 19$。

