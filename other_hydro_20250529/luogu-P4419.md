## 题目描述
Little Caesar likes card games. Everytime he comes to Zagreb, he plays blackjack, the famous card game, with his friends.

In this game, the player draws cards while the sum of the cards in his hand is less than or equal to 21 or until he says “DOSTA” (Croatian for “STOP”).

At the beginning of the game, there are 52 cards in the deck, thirteen ranks of each of the four suits. The card ranks are two, three, …, ten, Jack, Queen, King and Ace. The card values are the following: the cards with numbers on them are worth that number (e.g., “nine” is 9), the cards with pictures (Jack, Queen, and King) are worth 10, whereas the Ace is worth 11.

Caesar has found himself in an interesting situation. During the game, he already drew N cards whose sum is less than or equal to 21 and is now having second thoughts about drawing one more card or not. Let’s assume X is the difference from the sum of the cards so
far to 21. Everybody knows that you don’t draw a card if the number of the remaining cards in the deck whose value is greater than X is greater than or equal to the number of the remaining cards in the deck whose value is less than or equal to X.

Since Caesar is having a difficult time calculating whether he needs to draw another card or not, he’s asking you to do it for him.


## 输入格式
The first line of input contains the positive integer N (1 ≤ N ≤ 52), the number of cards Caesar has drawn so far.

Each of the following N lines contains a single positive integer, the value of the $i^{th}$ card Caesar drew.

## 输出格式
If Caesar should draw another card, output “VUCI” (Croatian for “DRAW”), otherwise output “DOSTA” (Croatian for “STOP”).

## 题目大意
小凯撒喜欢玩纸牌游戏，每次他去萨格勒布（克罗地亚的首都 ——译者注）都会和他的朋友们玩 $21$ 点，这是一种很流行的纸牌游戏。

这个游戏的规则是，在纸牌点数之和小于 $21$ 点之前可以连续抓牌，如果决定不抓牌，则喊 `DOSTA`（克罗地亚语“停止”的意思）。

游戏开始时，桌面有 $52$ 张牌 —— $13$ 种不同牌面的牌，每种有 $4$ 个花色。牌面分别是 $2,3,\dots,\text J,\text Q,\text K,\text A$。它们的点数计算规则是：牌面上的数字就是点数（比如，$9$ 的点数就是 $9$），特殊地，$\text J,\text Q,\text K$ 都算 $10$ 点，$\text A$ 算 $11$ 点。

凯撒认为游戏的乐趣在于，当抓了 $N$ 张牌之后，如果点数之和小于或等于 $21$，他就要思考是否要再多抓一张。假设 $X$ 是已抓牌点数之和与 $21$ 之间相差的点数值，我们知道，如果桌面上的剩余牌中点数大于 $X$ 的纸牌数量比小于等于 $X$ 的纸牌数量要多，或两者一样多，那就不应该再抓牌了。

因为凯撒并不擅于计算是否需要抓牌，所以他请你帮他计算和决策。

**【输入格式】**

第一行输入一个正整数 $N$（$1 \le N \le 52$），表示凯撒已经抓牌的张数。

接下来 $N$ 行每行一个正整数，第 $i$ 个正整数是他抓的第 $i$ 张牌点数值。

**【输出格式】**

如果凯撒应该继续抓牌，输出 `VUCI`（克罗地亚语“抓牌”的意思），否则输出 `DOSTA`（克罗地亚语“停止”的意思）。

**【样例解释】**

第一个样例： 已经抓的 $6$ 张牌的总点数是 $15$，它与 $21$ 的差 $X$ 是 $6$。桌面上剩余牌中比 $6$ 大的牌有 $32$ 张（分别是 $4$ 张 $\text A$、$4$ 张 $\text K$、$4$ 张 $\text Q$、$4$ 张 $\text J$、$4$ 张 $10$、$4$ 张 $9$、$4$ 张 $8$、$4$ 张 $7$），而比 $6$ 小的牌有 $14$ 张（分别是 $1$ 张 $2$、$1$ 张 $3$、$4$ 张 $4$、$4$ 张 $5$、$4$ 张 $6$），所以决定不再抓牌，输出 `DOSTA`。

```input1
6
2
3
2
3
2
3

```

```output1
DOSTA 
```

```input2
1
10

```

```output2
VUCI
```

```input3
2
5
6
```

```output3
VUCI
```

## 提示
Clarification​ ​of​ ​the​ ​first​ ​test​ ​case:

The sum of the already drawn cards is 15, and the difference X to 21 is 6. The number of cards in the
deck with a value greater than 6 is 32 (4 Aces, 4 Kings, 4 Queens, 4 Jacks, 4 tens, 4 nines, 4 eights, and 4 sevens), whereas the number of cards in the deck with a value less than or equal to 6 is 14 (one two, one three, 4 fours, 4 fives, and 4 sixes).

