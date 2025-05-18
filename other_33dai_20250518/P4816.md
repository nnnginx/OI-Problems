## 题目描述
Bessie the cow is a huge fan of card games, which is quite surprising, given her lack of opposable thumbs. Unfortunately, none of the other cows in the herd are good opponents. They are so bad, in fact, that they always play in a completely predictable fashion! Nonetheless, it can still be a challenge for Bessie to figure out how to win.

Bessie and her friend Elsie are currently playing a simple card game where they take a deck of $2N$ cards, conveniently numbered $1…2N$, and divide them into $N$ cards for Bessie and $N$ cards for Elsie. The two then play $N$ rounds, where in each round Bessie and Elsie both play a single card. In the first $N/2$ rounds, the player with the highest card earns a point, and in the last $N/2$ rounds, the rules switch and the player who plays the lowest card wins a point.

Given that Bessie can predict the order in which Elsie will play her cards, please determine the maximum number of points Bessie can win. 

## 输入格式
The first line of input contains the value of $N$ ($2 ≤ N ≤ 50,000$; N will be even).

The next $N$ lines contain the cards that Elsie will play in each of the successive rounds of the game. Note that it is easy to determine Bessie's cards from this information. 

## 输出格式
 Output a single line giving the maximum number of points Bessie can score. 

## 题目大意
### 题目描述

奶牛 Bessie 是卡牌游戏的狂热爱好者，尽管她没有对生拇指，但这并不影响她的热情。遗憾的是，她的同伴们在卡牌游戏方面水平堪忧，甚至出牌顺序都完全可预测！尽管如此，Bessie 仍需精心策划才能获胜。

Bessie 和她的朋友 Elsie 正在玩一个简单的卡牌游戏。她们使用一副包含 $2N$ 张卡牌的牌组（编号为 $1 \ldots 2N$），并将牌分成各 $N$ 张。随后进行 $N$ 轮比赛：每轮双方各打出一张牌。在前 $N/2$ 轮中，打出较大数字的玩家得 1 分；在后 $N/2$ 轮中，规则反转，打出较小数字的玩家得 1 分。

已知 Bessie 可以预知 Elsie 每轮出牌的顺序，请计算 Bessie 能够获得的最大分数。

### 输入格式

第一行输入包含整数 $N$（$2 \leq N \leq 50,000$，且 $N$ 为偶数）。

接下来 $N$ 行按顺序给出 Elsie 在每轮比赛中将打出的卡牌。注意根据这些信息可以推断出 Bessie 手中的卡牌。

### 输出格式

输出一行，包含 Bessie 能够获得的最大分数。

### 说明/提示

在此样例中，Bessie 手中的卡牌为 $2$、$5$、$6$ 和 $7$。她可以通过在比赛后半段保留 $2$ 这张牌，从而最多获得 2 分。

题目提供者：Brian Dean

```input1
4
1
8
4
3

```

```output1
2
```

## 提示
Here, Bessie must have cards 2, 5, and 6, and 7 in her hand, and she can use these to win at most 2 points, by saving her '2' card until one of the hands in the second half of the game.

Problem credits: Brian Dean 

