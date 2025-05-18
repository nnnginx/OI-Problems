## 题目背景
译自 [Potyczki Algorytmiczne 2016](https://sio2.mimuw.edu.pl/c/pa-2016-1/p/) R1 Gra w karty [A] (KAR)。$\texttt{1s,256M}$。


## 题目描述

Alice 和 Bob 各有 $n$ 张卡牌。每个人的卡牌都被编号为 $1\sim n$。

现在玩 $(n-1)$ 局游戏：每局游戏中，Alice 先弃掉 Bob 的一张牌，然后 Bob 再弃掉 Alice 的一张牌。

最终两人都只剩下一张牌。

有 $m$ 对关系，形如「若 Alice 最后剩下的牌为 $x$，Bob 最后剩下的牌为 $y$，则 Alice 胜/负 Bob」。特别地，未给出的关系为平局。

若双方都用最优策略游戏，Alice 最终会胜/负 Bob 还是平局？

「最佳策略」指的是：若有必胜策略，则选择必胜策略；否则若有平局策略，选择平局策略。

## 输入格式

**本题单个测试点内有多组测试数据。**

第一行，一个正整数 $T$。接下来描述 $T$ 组测试数据：

每组数据第一行，两个整数 $n,m$。

接下来 $m$ 行，每行两个正整数和一个字符 $x,w,y$，其中 $w\in \{\texttt{<},\texttt{>}\}$，$x,y$ 为正整数。
- 若 $w=\texttt{>}$，则表示「若 Alice 最后剩下的牌为 $x$，Bob 最后剩下的牌为 $y$，则 Alice 胜 Bob」；
- 若 $w=\texttt{<}$，则表示「若 Alice 最后剩下的牌为 $x$，Bob 最后剩下的牌为 $y$，则 Alice 负 Bob」。

保证不会出现自相矛盾的关系。


## 输出格式

输出 $T$ 行，每行一个字符串：
- 若 Alice 有必胜策略，输出 $\texttt{WYGRANA}$；
- 否则，若 Alice 有平局策略，输出 $\texttt{REMIS}$；
- 否则，输出 $\texttt{PRZEGRANA}$。


```input1
3
5 5
5 > 5
1 > 5
3 > 5
4 > 5
2 > 5
2 2
1 > 1
1 > 2
1 1
1 < 1
```

```output1
WYGRANA
REMIS
PRZEGRANA
```

## 提示

- $1\le T\le 20$；
- $1\le n\le 10^5$；
- $0\le m\le 2\times 10^5$；
- $1\le x,y\le n$；
- $w\in \{\texttt{<},\texttt{>}\}$。

保证不会出现自相矛盾的关系，也不会重复给出一个关系。

