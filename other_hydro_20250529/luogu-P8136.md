## 题目背景
ICPC2020 WF I

## 题目描述
To relax before competing in the ICPC World Finals, you have decided to play a
computer game called *Quests*. You have played it a
number of times already, and now you want to achieve a perfect
playthrough---to prepare for your perfect playthrough of the finals!

In the game, you have to complete a number
of quests, and you earn experience points (XPs) for completing each one. The
total number of XPs you have earned at any time determines your current level. You
reach a new level for every $v$ XPs that you earn. Formally, your level at
any time is the largest integer $L$ such that you have at least $L \cdot v$
XPs.

Each quest is assigned a number $x$ of XPs and a target
difficulty level $d$. If you complete the quest when your level is at least
$d$, you earn $x$ XPs. However, if you complete the quest when your level is
less than $d$, you will earn $c \cdot x$ XPs. The constant  $c$ is an XP multiplier
that results in a bonus for completing a
quest when you are at a lower level than the recommended level $d$.

You know all the $n$ quests and their respective $x$ and $d$ numbers by heart
(and you know the numbers $v$ and $c$ as well---you have played this game a lot).
You are also skilled enough to
complete any quest, regardless of its target difficulty level and your level.
You want to complete all the quests in an order that will allow you
to earn the largest possible number of XPs.

For example in the sample input, the maximum XPs you can earn is 43, which
is done as follows. First complete the second quest (you earn $4$ XPs,
because you are at level $0$, and you completed a quest with target difficulty
level $2$). Then complete the first quest (you earn $30$ XPs, because you are
still at level $0$, and the target difficulty level is $1$). With $34$ XPs, you
are now level $3$. Finally, complete the third quest (for which you earn $9$
XPs, without the multiplier, since you are already at level $3$).

## 输入格式
The first line of input contains three integers $n$, $v$, and $c$, where
$n$ $(1 \leq n \leq 2\,000)$ is the number of quests in the game, $v$
$(1 \leq v \leq 2\,000)$ is the number of XPs required to reach each level,
and $c$ $(2 \leq c \leq 2\,000)$ is the XP multiplier for completing a quest
before reaching its target difficulty level.

Following that are $n$ lines, each of which contains two integers $x$ and $d$
describing one quest, where $x$ $(1 \leq x \leq 2\,000)$ is the number of XPs
you earn for completing that quest if you are at or above its target difficulty
level and $d$ $(1 \leq d_i \leq 10^6)$ is the target difficulty level for that
quest.

## 输出格式
Output the maximum possible number of XPs you could earn by finishing all the
quests.

## 题目大意
为了在 ICPC 之前放松，小 A 决定玩一个名叫 _Quests_ 的游戏。你之前已经玩了很多次，因此这次你决定打一盘最完美的游戏——为你在决赛中的完美表现作准备！

游戏中你需要完成若干个任务，完成每一个任务都可以积攒经验值。你在某一时刻积攒的在总经验值决定了你的游戏等级，具体地，每次达到一个新的等级需要 $v$ 点经验值，也就是说，假设你在某一时刻积攒的总经验值为 $X$，那么你在该时刻的等级就是最大的满足 $L\cdot v\leqslant X$ 的整数 $L$。

游戏中的第 $i$ 个任务的设定经验值为 $x_i$，参考难度为 $d_i$。如果你在等级 $\geqslant d_i$ 的情况下完成了第 $i$ 个任务，那么你将获得 $x_i$ 点经验值。然而，如果你在等级 $<d_i$ 的情况下完成了第 $i$ 个任务，那么你将获得 $c\cdot x_i$ 点经验值。

现在，你已经知道了 $v,c$ 的值以及所有任务的设定经验值 $x_i$ 和参考难度 $d_i$，你想知道在按照某一特定顺序依次完成任务的情况下，能够攒到的总经验值最大是多少。

数据范围：

- $1\leqslant n,v\leqslant 2000$，$2\leqslant c\leqslant 2000$。
- $1\leqslant x_i\leqslant 2000$，$1\leqslant d\leqslant 10^6$。

Translated by Eason_AC

```input1
3 10 2
15 1
2 2
9 1
```

```output1
43
```

