## 题目描述
Byteasar the hacker has qualified for this year’s IHO, the International Hacking Olympiad. One of the tasks in the Olympiad involves competing against a system operator. There are $n$ computers numbered from $1$ to $n$,connected in a ring topology, i.e. computers $i$ and $i+1$ are connected $(for \ i = 1,...,n-1)$, and also computers $n$ and $1$ are connected.
The competition is performed as a game between the hacker and the system operator:
   - Byteasar moves first. Afterwards, the operator and Byteasar move alternately.
   - In his first move, Byteasar chooses any computer and hacks it (for instance,by exploiting some operating system vulnerabilities).
   - In his first move, the operator chooses any non-hacked computer and protects it (for instance, by installing latest security upgrades).
   - In all his following moves, Byteasar either (a) does nothing or (b) chooses any computer that is neither hacked nor protected and is directly linked to any hacked computer, and hacks it.
   - In all his following moves, the operator either (a) does nothing or (b) chooses any computer that is neither hacked nor protected and is directly linked to any protected computer, and protects it.
   - The game ends as soon as both have done nothing in two subsequent moves.

At the beginning of the game none of the computers are hacked or protected.
Every computer $i$ has a certain value viwhich specifies the value of the data which is stored on it. For each hacked computer $i$, Byteasar scores its value $v_i$. Byteasar is quite a good hacker, but has no idea of algorithms.
That is why he asks you to write a program that computes his maximum possible score, assuming that the operator plays optimally.

## 输入格式
The first line of input contains a positive integer $n(n \ge 2)$, specifying the number of computers. The second line contains a sequence of $n$ integers $v_1,v_2,...,v_n(1 \le v_i \le 2000)$; number vispecifies the value of the data
stored on computer $i$.

## 输出格式
In the first and only line of output your program should write one integer: Byteasar’s maximum possible score against an optimally playing operator.

## 题目大意
### 题面描述

Byteasar 获得了今年国际黑客奥林匹克竞赛的参赛资格。竞赛的任务之一是与系统操作员竞争。有从 $1$ 到 $n$ 编号的 $n$ 台计算机，以环形连接，即计算机 $i$ 和 $i+1$ 连接（其中 $i = 1,2,\dots,n-1$），特别地，计算机 $n$ 和 $1$ 也连接。

这个任务是黑客和系统操作员之间的游戏：

- Byteasar 先走。之后，操作员和 Byteasar 交替移动。
- Byteasar 的第一步是选择任何一台计算机并对其进行黑客攻击。
- 在他的第一步中，操作员选择任何未被黑客攻击的计算机并对其进行保护。
- 在接下来的所有动作中，Byteasar 要么什么都不做，要么选择任何既没有被黑客攻击也没有受到保护的计算机，并直接链接到任何被黑客攻击的计算机，然后对其进行黑客攻击。
- 在接下来的所有动作中，操作员要么什么都不做，要么选择任何既没有被黑客攻击也没有受到保护的计算机，直接链接到任何受保护的计算机并对其进行保护。
- 一旦两人在接下来的两个动作中都没有做任何事情，游戏就结束了。

在游戏开始时，没有任何一台电脑被黑客攻击或受到保护。

每台计算机 $i$ 都有一个特定的值 $v_i$，该值指定了存储在其上的数据的价值。Byteasar 最终获得的分数就是所有被他攻击的计算机的 $v$ 值之和。

虽然 Byteasar 是一个很好的黑客，但对算法一无所知——这就是为什么他要求你编写一个程序来计算他的最大可能分数，假设操作员按最优策略。

### 输入格式
第一行输入包含一个正整数 $n(n\ge 2)$，指定计算机的数量。第二行包含一个含有 $n$ 个整数的序列 $v_1,v_2,\dots,v_n(1\le v_i\le 2000)$。

### 输出格式

在输出的第一行，也是唯一一行，你的程序应该输出一个整数：Byteasar 获得的总得分的最大值。

```input1
4
7 6 8 4
```

```output1
13
```

```input2
5
1 1 1 1 1
```

```output2
3
```

## 提示
**Explanation to the examples:** In the first example, Byteasar in his first move should hack computer $2$(scoring $6$). The operator’s response will be protecting computer $3$. In the next move Byteasar can hack computer $1$ (scoring $7$). Finally, the operator will protect computer $4$.

以下子任务与评测无关，仅供参考。

![PVIZHx.png](https://s1.ax1x.com/2018/07/05/PVIZHx.png)

