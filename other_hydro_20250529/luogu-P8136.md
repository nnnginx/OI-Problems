## ��Ŀ����
ICPC2020 WF I

## ��Ŀ����
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

## �����ʽ
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

## �����ʽ
Output the maximum possible number of XPs you could earn by finishing all the
quests.

## ��Ŀ����
Ϊ���� ICPC ֮ǰ���ɣ�С A ������һ������ _Quests_ ����Ϸ����֮ǰ�Ѿ����˺ܶ�Σ��������������һ������������Ϸ����Ϊ���ھ����е�����������׼����

��Ϸ������Ҫ������ɸ��������ÿһ�����񶼿��Ի��ܾ���ֵ������ĳһʱ�̻��ܵ����ܾ���ֵ�����������Ϸ�ȼ�������أ�ÿ�δﵽһ���µĵȼ���Ҫ $v$ �㾭��ֵ��Ҳ����˵����������ĳһʱ�̻��ܵ��ܾ���ֵΪ $X$����ô���ڸ�ʱ�̵ĵȼ������������� $L\cdot v\leqslant X$ ������ $L$��

��Ϸ�еĵ� $i$ ��������趨����ֵΪ $x_i$���ο��Ѷ�Ϊ $d_i$��������ڵȼ� $\geqslant d_i$ �����������˵� $i$ ��������ô�㽫��� $x_i$ �㾭��ֵ��Ȼ����������ڵȼ� $<d_i$ �����������˵� $i$ ��������ô�㽫��� $c\cdot x_i$ �㾭��ֵ��

���ڣ����Ѿ�֪���� $v,c$ ��ֵ�Լ�����������趨����ֵ $x_i$ �Ͳο��Ѷ� $d_i$������֪���ڰ���ĳһ�ض�˳������������������£��ܹ��ܵ����ܾ���ֵ����Ƕ��١�

���ݷ�Χ��

- $1\leqslant n,v\leqslant 2000$��$2\leqslant c\leqslant 2000$��
- $1\leqslant x_i\leqslant 2000$��$1\leqslant d\leqslant 10^6$��

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

