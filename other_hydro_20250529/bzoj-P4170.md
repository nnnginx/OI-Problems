本题与 [](/d/bzoj/p/2989) 相同。

## 题目背景

“若是万一琪露诺（俗称 rhl）进行攻击，什么都好，冷静地回答她的问题来吸引她。对方表现出兴趣的话，那就慢
慢地反问。在她考虑答案的时候，趁机逃吧。就算是很简单的问题，她一定也答不上来。”——《上古之魔书》

## 题目描述

天空中出现了许多的北极光，这些北极光组成了一个长度为 $n$ 的正整数数列 $a_i$，远古之魔书上记载到：两个位置的 $\operatorname{graze}$ 值为两者位置差与数值差的和：$\operatorname{graze}(x,y)=|x-y|+|a_x-a_y|$。

要想破解天罚，就必须支持两种操作（$k$ 都是正整数）：

1. `Modify x k`，表示将第 $x$ 个数的值修改为 $k$；
2. `Query x k`，表示询问有几个 $i$ 满足 $\operatorname{graze}(x,i)\leq k$。

由于从前的天罚被圣王 lmc 破解了，所以 rhl 改进了她的法术，询问不仅要考虑当前数列，还要考虑任意历史版本，即统计任意位置上出现过的任意数值与当前的 $a_x$ 的 $\operatorname{graze}$ 值 $\leq k$ 的对数。（某位置多次修改为同样的数值，按多次统计。）

## 输入格式

第一行两个整数 $n,q$。分别表示数列长度和操作数。

第二行 $n$ 个正整数，代表初始数列。

第 $3\sim q+2$ 行每行一个操作。

## 输出格式

对于每次询问操作，输出一个非负整数表示答案。

```input1
3 5
2 4 3
Query 2 2
Modify 1 3
Query 2 2
Modify 1 2
Query 1 1
```

```output1
2
3
3
```

## 数据范围

对于所有数据，保证 $n\leq 6\times 10^4$，修改操作数 $\leq 5\times 10^4$，询问操作数 $\leq 6\times 10^4$，$a_i$ 的所有历史版本的最大值 $\leq 10^5$。