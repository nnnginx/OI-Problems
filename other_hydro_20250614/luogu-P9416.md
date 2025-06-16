## 题目背景
译自 [XXIX Olimpiada Informatyczna – I etap](https://sio2.mimuw.edu.pl/c/oi29-1/dashboard/) [Domino](https://sio2.mimuw.edu.pl/c/oi29-1/p/dom/)。

## 题目描述
> 有一个 $2$ 行 $n$ 列的矩形，上面有若干个格子被占用了。你要用 $1\times 2$ 或 $2\times 1$ 的牌，覆盖所有未被占用的格子，一个格子不可被占用两次。记方案数为 $m$。

给你 $m$，求出最小的 $n$，使得存在一种方案设置占用格，使得覆盖的方案数恰好为 $m$。无解输出 `NIE`。

## 输入格式
一行一个正整数 $m$。

## 输出格式
如果有解，输出你的答案 $n$。

如果无解，输出 `NIE`。

```input1
4

```

```output1
5

```

```input2
101

```

```output2
NIE

```

```input3
9

```

```output3
7

```

```input4
11

```

```output4
NIE

```

```input5
500

```

```output5
20

```

```input6
112233445566778899

```

```output6
NIE

```

## 提示
对于所有数据，$1\leq m\leq 10^{18}$。

| 子任务编号 | 附加限制 | 分数 |
| :----------: | :----------: | :----------: |
| 1 | 答案 $\leq 12$ | 20 |
| 2 | $m\leq 2000000$ | 30 |
| 3 |  | 50 |

