## 题目描述
Every year, Farmer John brings his $N$ cows to compete for "best in show" at the state fair. His arch-rival, Farmer Paul, brings his $M$ cows to compete as well ($1 \leq N \leq 1000, 1 \leq M \leq 1000$).

Each of the $N + M$ cows at the event receive an individual integer score. However, the final competition this year will be determined based on teams of $K$ cows ($1 \leq K \leq 10$), as follows: Farmer John and Farmer Paul both select teams of $K$ of their respective cows to compete. The cows on these two teams are then paired off: the highest-scoring cow on FJ's team is paired with the highest-scoring cow on FP's team, the second-highest-scoring cow on FJ's team is paired with the second-highest-scoring cow on FP's team, and so on. FJ wins if in each of these pairs, his cow has the higher score.

Please help FJ count the number of different ways he and FP can choose their teams such that FJ will win the contest. That is, each distinct pair (set of $K$ cows for FJ, set of $K$ cows for FP) where FJ wins should be counted. Print your answer modulo 1,000,000,009.


## 输入格式
The first line of input contains $N$, $M$, and $K$. The value of $K$ will be no larger than $N$ or $M$.

The next line contains the $N$ scores of FJ's cows.

The final line contains the $M$ scores of FP's cows.


## 输出格式
Print the number of ways FJ and FP can pick teams such that FJ wins, modulo 1,000,000,009.


## 题目大意
### 题目描述

每年，Farmer John 都会带着他的 $N$ 头奶牛参加州展览会的“最佳展示”比赛。他的劲敌 Farmer Paul 也会带着他的 $M$ 头奶牛参加比赛（$1 \leq N \leq 1000, 1 \leq M \leq 1000$）。

参加比赛的每头 $N + M$ 头奶牛都会获得一个单独的整数得分。然而，今年的最终比赛将由 $K$ 头奶牛组成的团队决定（$1 \leq K \leq 10$），规则如下：Farmer John 和 Farmer Paul 各自选择 $K$ 头奶牛组成团队进行比赛。这两个团队的奶牛将按得分高低配对：FJ 团队中得分最高的奶牛与 FP 团队中得分最高的奶牛配对，FJ 团队中得分第二高的奶牛与 FP 团队中得分第二高的奶牛配对，依此类推。如果在每一对中，FJ 的奶牛得分都更高，那么 FJ 获胜。

请帮助 FJ 计算他和 FP 可以选择团队的不同方式的数量，使得 FJ 能够赢得比赛。也就是说，每个不同的（FJ 的 $K$ 头奶牛集合，FP 的 $K$ 头奶牛集合）对，只要 FJ 获胜，都应被计入。输出结果对 $1\,000\,000\,009$ 取模。

### 输入格式

输入的第一行包含 $N$、$M$ 和 $K$。$K$ 的值不会超过 $N$ 或 $M$。

第二行包含 FJ 的 $N$ 头奶牛的得分。

第三行包含 FP 的 $M$ 头奶牛的得分。

### 输出格式

输出 FJ 和 FP 可以选择团队的方式数量，使得 FJ 获胜，结果对 $1\,000\,000\,009$ 取模。

```input1
10 10 3
1 2 2 6 6 7 8 9 14 17
1 3 8 10 10 16 16 18 19 19
```

```output1
382
```

