## 题目描述
Bessie the cow is a hu e fan of card games, which is quite surprising, given her lack of opposable thumbs. Unfortunately, none of the other cows in the herd are good opponents. They are so bad, in fact, that they always play in a completely predictable fashion! Nonetheless, it can still be a challenge for Bessie to figure out how to win.

Bessie and her friend Elsie are currently playing a simple card game where they take a deck of $2N$ cards, conveniently numbered $1 \ldots 2N$, and divide them into $N$ cards for Bessie and $N$ cards for Elsie. The two then play $N$ rounds, where in each round Bessie and Elsie both play a single card. Initially, the player who plays the highest card earns a point. However, at one point  during the game, Bessie can decide to switch the rules so that for the rest of the game, the player who plays the lowest card wins a point.  Bessie can choose not to use this option, leaving the entire game in "high card wins" mode, or she can even invoke the option right away, making the entire game follow the "low card wins" rule.

Given that Bessie can predict the order in which Elsie will play her cards, please determine the maximum number of points Bessie can win.

## 输入格式
The first line of input contains the value of N ($2 \leq N \leq 50,000$).

The next N lines contain the cards that Elsie will play in each of the successive rounds of the game.  Note that it is easy to determine Bessie's cards from this information.

## 输出格式
Output a single line giving the maximum number of points Bessie can score.


## 题目大意
### 题目描述

奶牛 Bessie 是卡牌游戏的狂热爱好者，这相当令人惊讶，因为她没有灵活的手指。不幸的是，牛群中的其他奶牛都不是好的对手。事实上，她们的表现非常糟糕，总是以完全可预测的方式出牌！尽管如此，对 Bessie 来说，如何获胜仍然是一个挑战。

Bessie 和她的朋友 Elsie 正在玩一个简单的卡牌游戏。她们拿一副 $2N$ 张牌，方便地编号为 $1 \ldots 2N$，并将其分成 $N$ 张牌给 Bessie 和 $N$ 张牌给 Elsie。然后，两人进行 $N$ 轮游戏，每轮 Bessie 和 Elsie 各打出一张牌。最初，打出更高牌的玩家得一分。然而，在游戏中的某个时刻，Bessie 可以决定改变规则，使得在接下来的游戏中，打出更低牌的玩家得一分。Bessie 可以选择不使用这个选项，让整个游戏保持在“高牌获胜”模式，或者她也可以立即启用这个选项，让整个游戏遵循“低牌获胜”的规则。

已知 Bessie 可以预测 Elsie 出牌的顺序，请确定 Bessie 可以获得的最大分数。

### 输入格式

输入的第一行包含 $N$ 的值（$2 \leq N \leq 50,000$）。

接下来的 $N$ 行包含 Elsie 在游戏每轮中将要打出的牌。注意，从这些信息中可以很容易地确定 Bessie 手中的牌。

### 输出格式

输出一行，表示 Bessie 可以获得的最大分数。

### 说明/提示

在这里，Bessie 手中的牌必须是 2、5、6 和 7，她最多可以利用这些牌赢得 3 分。例如，她可以先击败 1 这张牌，然后将规则切换为“低牌获胜”，之后她可以再赢得两轮。

```input1
4
1
8
4
3
```

```output1
3
```

## 提示
Here, Bessie must have cards 2, 5, and 6, and 7 in her hand, and she can use these to win at most 3 points.  For example, she can defeat the 1 card and then switch the rules to "low card wins", after which she can win two more rounds.

