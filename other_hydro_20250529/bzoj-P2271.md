## 题目描述

Just like every fall，the organizers of the Southwestern Europe Dice Simulation Contest are busy again this year．In this edition you have to simulate a 3-sided die that outputs each of three possible outcomes （which will be denoted by $1,2$ and $3$） with a given probability，using three dice in a given set．The simulation is performed this way：you choose one of the given dice at random，roll it，and report its outcome．You are free to choose the probabilities of rolling each of the given dice，as long as each probability is strictly greater than zero．Before distributing the materials to the contestants，the organizers have to verify that it is actually possible to solve this task．

For example，in the first test case of the sample input you have to simulate a die that yields outcome $1,2$ and $3$ with probabilities，and．We give you three dice，and in this case the $i$-th of them always yields outcome $i$，for each $i = 1,2,3$．Then it is possible to simulate the given die in the following fashion：roll the first die with probability，the second one with probability and the last one with probability．

一个骰子有 $3$ 个面，$3$ 个面（$A,B,C$ 面）上分别有 $3$ 个数字。在本题中，先给出了 $3$ 个骰子，每个骰子给出 $3$ 个面的数字。我们保证对于每个骰子，$3$ 个面的数字和为 $1 \times 10^4$。之后再给出一个我们希望得到的 $A,B,C$ 面的结果，然后希望你给 $3$ 个骰子分配概率， 第一个骰子分配概率 $p_1$，第二个 $p_2$，第三个 $p_3$，满足：

1. $p_1 + p_2 + p_3 = 1$

2. $3$ 个骰子的每个面的期望和等于给出的那个面的期望的和

例如，样例1中：

```
0 0 10000

0 10000 0

10000 0 0
```

骰子1：$A(0)$，$B(0)$，$C(10000)$；

骰子2：$A(0)$，$B(10000)$，$C(0)$；

骰子3：$A(10000)$，$B(0)$，$C(0)$。

目标：$A(3000)$，$B(4000)$，$C(3000)$。

于是我可以分配 $p_1={3} \over {10}$，$p_2={4} \over {10}$，$p_3={3} \over {10}$。

这样

$A$ 面期望: $p_1 \times 0 + p_2 \times 0 + p_3 \times 10000 = 3000$

$B$ 面期望: $p_1 \times 0 + p_2 \times 10000 + p_3 \times 0 = 4000$

$C$ 面期望: $p_1 \times 10000 + p_2 \times 0 + p_3 \times 0 = 3000$

在本题中，保证给出的 $3$ 个数对的和均为 $10000$。

## 输入格式

**本题有多组数据**

The input consists of several test cases，separated by single blank lines．Each test case consists of four lines：

the first three of them describe the three dice you are given and the last one describes the die you have to simulate．

Each of the four lines contains $3$ space-separated integers between $0$ and $10000$ inclusive．These numbers will add up to $10000$，and represent $10000$ times the probability that rolling the die described in that line yields outcome $1，2$ and $3$，respectively．

The test cases will finish with a line containing only the number zero repeated three times （also preceded with a blank line）．

输入多组数据，每组数据给出 $3$ 个骰子的 $A，B，C$ 面的点数，然后给出一个期望的结果。

保证给出的 $3$ 个数对的和均为 $10000$。

如果遇到 $3$ 个 $0$，那么则表示数据结束

## 输出格式

For each case，your program should output a line with the word `YES` if it is feasible to produce the desired die from the given ones，and `NO` otherwise．
对于期望的数对，如果可以分配 $p_1,p_2,p_3$ 满足以上条件，则输出 `YES` 否则输出 `NO`。

```input1
0 0 10000
0 10000 0
10000 0 0
3000 4000 3000
0 0 10000
0 10000 0
3000 4000 3000
10000 0 0
0 0 0
```

```output1
YES
NO
```

## 题目来源

鸣谢 AekdyCoin