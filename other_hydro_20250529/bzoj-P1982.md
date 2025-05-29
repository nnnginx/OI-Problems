## 题目描述

Two players play the following game. At the beginning of the game they start with $n$ piles of stones. At each step of the game, the player chooses a pile and remove at least one stone from this pile and move zero or more stones from this pile to any other pile that still has stones. A player loses if he has no more possible moves. Given the initial piles, determine who wins: the first player, or the second player, if both play perfectly.

给你 $n$ 堆石子，两个人玩游戏。每次任选一堆，首先拿掉至少一个石头，然后移动任意个石子到任意堆中。谁不能移动了，谁就输了。

## 输入格式

Each line of input has one integer $n$, followed by $n$ positive integers denoting the initial piles.

## 输出格式

For each line of input, output `first player` if first player can force a win, or `second player`, if the second player can force a win.

```input1
3 2 1 3
```

```output1
first player
```

## 数据规模与约定

对于 $100\%$ 的数据，$1 \le n \le 10^5$。