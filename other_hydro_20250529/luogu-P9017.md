## 题目描述
**Note: The time limit for this problem is 4s, twice the default.**

Bessie wants to go to sleep, but the farm's lights are keeping her awake. How can she turn them off?

Bessie has two bit strings of length $N
(2 \le N \le 20)$, representing a sequence of lights and a sequence of switches, respectively. Each light is either on (1) or off (0). Each switch is either active (1) or inactive (0).

A **move** consists of the following sequence of operations: 

1. Toggle exactly one switch (set it to active if it is inactive, or vice versa).
2. For each active switch, toggle the state of the corresponding light (turn it off if it is on, or vice versa).
3. Cyclically rotate the switches to the right by one. Specifically, if the bit string corresponding to the switches is initially $s_0s_1\cdots s_{N−1}$ then it becomes $s_{N−1}s_0s_1 \cdots s_{N−2}$.

For $T (1 \le T \le 2 \cdot 10^5)$ instances of the problem above, count the minimum number of moves required to turn all the lights off. 

## 输入格式
First line contains $T$ and $N$.

Next $T$ lines each contain a pair of length-$N$ bit strings. 

## 输出格式
 For each pair, the minimum number of moves required to turn all the lights off. 

## 题目大意
### 题目描述

给定正整数 $N$，和两个长为 $N$ 的 $01$ 序列 $a$ 和 $b$。定义一次操作为：

1. 将 $b$ 序列中的一个值翻转（即 $0$ 变成 $1$，$1$ 变成 $0$，下同）。
2. 对于 $b$ 序列中每个值为 $1$ 的位置，将 $a$ 序列中对应位置的值翻转。
3. 将 $b$ 序列向右循环移位 $1$ 位。即若当前 $b$ 序列为 $b_1b_2\cdots b_{n}$，则接下来变为 $b_{n}b_1b_2\cdots b_{n-1}$。

有 $T$ 次询问，对每一次询问，你需要回答出至少需要几次操作，才能使 $a$ 序列中每一个位置的值都变为 $0$。

### 输入格式

第一行为两个正整数 $T,N\;(1\leq T\leq 2\times10^5,2\leq N\leq 20)$。

接下来 $T$ 行，每行为两个长为 $N$ 的 $01$ 序列 $a$ 和 $b$，表示一组询问。

### 输出格式

共 $T$ 行，每行一个正整数，表示最少的操作次数。

```input1
4 3
000 101
101 100
110 000
111 000
```

```output1
0
1
3
2
```

```input2
1 10
1100010000 1000011000
```

```output2
2
```

## 提示
### Explanation for Sample 1

 - First test case: the lights are already all off.
 - Second test case: We flip the third switch on the first move.
 - Third test case: we flip the first switch on the first move, the second switch on the second move, and the second switch again on the third move.
 - Fourth test case: we flip the first switch on the first move and the third switch on the second move. 
 
It can be shown that in each case this is the minimal number of moves necessary. 

### Explanation for Sample 2

It can be shown that $2$ moves are required to turn all lights off.

 - We flip the seventh switch on the first move and then again on the second move. 
 
### Scoring

 - Inputs $3-5$: $N \le 8$
 - Inputs $6-13$: $N \le 18$
 - Inputs $14-20$: No additional constraints.

