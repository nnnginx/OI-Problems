# AT_s8pc_6_a E869120, who Leaps through Time

## 题目描述

E869120 居住在高桥王国。

他在 AtCodeer 公司工作。在这家公司，每天必须在 $0$ 点准时参加一个会议。

高桥王国有 $N$ 个城市，从西向东依次编号为城市 $1,2,3,\dots,N$。他的家在城市 $1$，而他的公司在城市 $N$。此外，高桥王国有连接城市 $i$ 和 $i+1(1 \leq i \leq N - 1)$ 的双向道路，通过这条道路移动需要 $A_i$ 分钟。注意，$1$ 分钟是从时间 $0$ 到时间 $1$ 的时间。

$2031$ 年的某一天... 他醒来检查时钟，发现竟然是时间 $0$！

如果这样下去，他会迟到。AtCodeer 公司对迟到非常严格，如果迟到一次，不仅仅是责备和减薪，很可能会直接被解雇！

但他拥有一种特殊能力，那就是“时间跳跃”。使用这个能力一次，时间会倒退 $T$ 分钟。他可以在任何城市使用“时间跳跃”。

为了不迟到，也就是说，要在时间 $0$ 或之前到达城市 $N$ 的公司，他至少需要使用多少次“时间跳跃”，请计算出来。

注意，他可以在醒来的时间 $0$ 开始行动。

## 输入格式

输入将以以下格式从标准输入中给出。

> $ N $ $ T $ $ A_1 $ $ A_2 $ $ A_3 $ ... $ A_{N\ -\ 1} $

## 输出格式

请在一行中输出他必须使用的“时间跳跃”的最小次数。

## 输入输出样例 #1

### 输入 #1

```
2 1
3
```

### 输出 #1

```
3
```

## 输入输出样例 #2

### 输入 #2

```
3 4
5 6
```

### 输出 #2

```
3
```

## 说明/提示

### 限制

- $N$ 是 $2$ 到 $100$ 之间的整数
- $T$ 是 $1$ 到 $100$ 之间的整数
- $A_i$ 是 $1$ 到 $100$ 之间的整数

### 部分得分

这个问题被分成了几个小任务，如果你的程序能正确处理所有为小任务准备的测试用例，你将获得该小任务的分数。

提交的源代码的得分是正确答案的小任务分数之和。

1. ($100$ 分)：$N = 2, T = 1$

2. ($100$ 分)：没有额外的限制

### 样例解释 1

例如，如果他采取以下行动，可以将“时间跳跃”的次数减少到 $3$ 次，这是最小的。

最初，E869120 在城市 $1$，时间是 $0$。

![](https://img.atcoder.jp/s8pc-6/caa13b096b89d11a1c57faa1d297a049.png)

在城市 $1$ 使用“时间跳跃”$3$ 次。此时，时间是 $-3$。

![](https://img.atcoder.jp/s8pc-6/1b592053466048d7201b2af72dbebe24.png)

从城市 $1$ 移动到城市 $2$。移动结束后，时间是 $0$，所以他刚好赶上！

![](https://img.atcoder.jp/s8pc-6/8787549cd3e039f2218cfab151a53642.png)

### 样例解释 2

请注意，这个输入示例不满足小任务 $1$ 的限制。