## 题目背景
可怜的小 Bronya，因为想不到好的 idea 气的又哭又闹，呜呜呜呜，好可怜啊。

## 题目描述
Bronya 想给《阿拉哈托·集训队互测》出个新的 DLC，但是想不到好的 idea。

她现在有 $n$ 个 idea，每个 idea 都有一个难度值 $a_i$，满足 $1 \leq a_i \leq m$。

她现在打算在这些 idea 中抽取一个 idea 作为最终 idea，她的抽取方式如下：

随机在 $\frac{n(n + 1)}{2}$ 个区间中，等概率抽取一个编号区间 $[l, r]$，然后再在 $[1, m]$ 中等概率抽取一个整数作为难度上限 $lim$，然后 Bronya 会在所有满足 $i \in [l, r], a_i \leq lim$ 的 $i$ 中选一个 $a_i$ 最大的 $i$ 作为 $x$。

此时 $a_x$ 会作为最终的难度值，若这样的 $x$ 不存在，那最终的难度值为 $0$。

Bronya 想知道最终难度值的期望，请你帮帮可爱的她。

由于期望是高贵的 10 级算法，小 Bronya 不会，所以请你输出期望乘以 $\frac{n \times (n + 1) \times m}{2}$ 的值。

## 输入格式
第一行两个整数 $n, m$，分别表示 idea 的数量和难度值的上限。

第二行 $n$ 个整数，第 $i$ 个整数 $a_i$ 表示第 $i$ 个 idea 的难度值。


## 输出格式
一行一个整数 $ans$，表示最终难度值的期望乘以 $\frac{n \times (n + 1) \times m}{2}$ 之后的值。

```input1
3 4
1 1 4
```

```output1
30
```

```input2
10 20
5 19 3 14 2 8 18 7 1 5
```

```output2
7535
```

## 提示
### 样例解释

考虑最后选出的区间有 $[1, 1], [1, 2], [1, 3], [2, 2], [2, 3], [3, 3]$ 六种可能。

其难度值期望分别是 $1, 1, \frac{7}{4}, 1, \frac{7}{4}, 1$，则最后的答案为 $\frac{1 + 1 + \frac{7}{4} + 1 + \frac{7}{4} + 1}{6} \times 6 \times 4 = 30$。

### 数据范围

对于所有测试点，$1 \leq n \leq 1 \times 10^6, 1 \leq m \leq 1 \times 10^9$。

- Subtask 1（5pts）：$n \leq 500$
- Subtask 2（5pts）：$n \leq 4000$，依赖 Subtask 1。
- Subtask 3（5pts）：$m \leq 2$。
- Subtask 4（20pts）：$m \leq 50$，依赖 Subtask 3。
- Subtask 5（10pts）：保证 $a_i$ 在 $[1, m]$ 中随机生成，$n \leq 5 \times 10^5$。
- Subtask 6（20pts）：$n \leq 10^5$，依赖 Subtask 1,2。
- Subtask 7（35pts）：无限制，依赖 Subtask 1,2,3,4,5,6。

Subtask 依赖暂未配置。

