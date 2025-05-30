## 题目描述


Debbie, Debby, Debra and Deborah are going to play a game with marbles together. Debbie has brought $2^{d_{1}}$ marbles, Debby -- $2^{d_{2}}$ marbles, Debra -- $2^{d3}$ marbles, while Deborah -- $2^{d4}$ marbles. The kids have gathered their marbles into a single pile containing $2^{d_{1}} + 2^{d_{2}} + 2^{d_{3}} + 2^{d_{4}}$ marbles, and the game is starting.

The game consists of turns. Each turn consists of two steps:

The kids choose any of their piles with more than one marble and divide it into two non-empty piles. That is, if the chosen pile contains $m \ge 2$ marbles, the new piles must contain $m_{1}$ and $m_{2}$ marbles where $m_1$ and $m_2$ are positive integers, and $m_{1} + m_{2} = m$ .

If there are several piles with the same number of marbles, only one of these piles is kept, while all the others with this number of marbles are discarded (thrown away).

The game ends when only one pile is left, and this pile contains a single marble. The goal of the game is to end it in the least possible number of turns. Note that the game is cooperative, that is, the kids aren't playing against each other, but trying to reach a common goal together.

Help the kids and find the best way to play.



## 输入格式


The first line of the input contains a single integer $T$ -- the number of test cases $(1 \le T \le 500)$ .

Each of the next $T$ lines describes one test case and contains four non-negative integers $d_{1}, d_{2}, d_{3}, d_{4} (0 \le d_{i} \le 20)$ .



## 输出格式


For each test case, output an integer $t$ -- the smallest number of turns required to end the game.

Then, output $t$ turn descriptions, in the order the turns should be made. Each description should consist of three integers $m , m_{1}, m_{2}$ -- the size of the divided pile and the sizes of the new piles, respectively $(m \ge 2$ ; $m_{1} > 0$ ; $m_{2} > 0$ ; $m_{1} + m_{2} = m)$ . Note that a pile of size $m$ must exist at that moment, and at the end of the game there should be only one pile left and that pile should contain a single marble.



## 题目大意
**题目描述**

Debbie, Debby, Debra 和 Deborah要一起玩一个关于弹珠的游戏。Debbie 带来了  $2^{d_{1}}$ 颗弹珠, Debby 带来了  $2^{d_{2}}$ 颗弹珠, Debra 带来了  $2^{d3}$ 颗弹珠, 而 Deborah 带来了  $2^{d4}$ 颗弹珠。这些孩子们把他们的弹珠放在一起，总共有 $2^{d_{1}} + 2^{d_{2}} + 2^{d_{3}} + 2^{d_{4}}$ 颗, 游戏开始了。

游戏是多回合制。每一个回合包括两个步骤：

这些孩子们选择他们的任意一堆大于1个的弹珠然后分入两个大于0个的堆中。相当于，如果选中的那堆有 $m \ge 2$ 颗弹珠, 新的一堆必须要有 $m_{1}$ 和 $m_{2}$ 颗弹珠且 $m_1$ 和 $m_2$ 为正整数, 且 $m_{1} + m_{2} = m$.

如果有许多堆拥有同样数目的弹珠，只有一堆会被保留，其他的都会被丢弃。

当只有一堆弹珠被留下且这堆弹珠只有一颗时，游戏就结束了。游戏的目标就是用尽量少的回合让游戏结束。注意这个游戏是合作性质的，那就是，这些孩子不是互相争斗的，而是一起尝试达成同一个目标。

请帮助这些孩子找到游戏的最佳方案。

**输入格式**

第一行包括一个单独的整数，T 即测试用例的数量$(1≤T≤500)$ .

下面的每一行都描述一个测试用例且包含四个非负整数 $d_{1}, d_{2}, d_{3}, d_{4} (0 \le d_{i} \le 20)$

**输出格式**

对于每一个测试用例，输出一个整数t，即游戏结束所需的最少次数。

然后，按照回合的顺序，输出这些回合的说明。每一行说明都要包括三个整数 $ m , m_{1}, m_{2}$ 即是被分的堆和新堆的弹珠数量，依次为$(m≥2 ; m_{1} > 0; m_{2} > 0 ;  m_{1} + m_{2} = m)$ 

请注意大小为m的弹珠堆一定要存在，且在游戏结束时应该只剩下一堆且那一堆应该只有一颗弹珠。

**说明/提示**

时间限制: 3 s, 内存限制: 512 MB.

```input1
2
1 0 1 0
0 1 2 3

```

```output1
3
6 2 4
4 2 2
2 1 1
5
15 10 5
10 5 5
5 1 4
4 2 2
2 1 1

```

## 提示
Time limit: 3 s, Memory limit: 512 MB. 



