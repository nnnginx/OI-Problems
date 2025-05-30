## 题目描述
![](https://cdn.luogu.com.cn/upload/image_hosting/kdojyok4.png)

Example placement of cards for $k = 5$

There is a fairly well-known mentalism trick known as the Fitch Cheney trick. From a deck of $n$ playing cards, $k$ are selected uniformly at random and given to an assistant while the magician is out of the room. The assistant places $k-1$ of the selected cards on a table, face up, and the single remaining card face down. The cards are placed in a single row with the face-down card at the end (see the picture for an example). The magician enters the room, looks at the cards on the table, and announces what the $k^{th}$ card is, although its face is hidden. The trick is typically done with $n=52$ and $k=5$.

The assistant uses two ways of passing information to the magician. First, they can pick which one of the $k$ cards to keep hidden. Second, they can rearrange the other $k-1$ cards in a specific way. For the case $n=52$ and $k=5$ both techniques are needed, since there are only $24$ ways of rearranging four cards, which is not enough to reliably signal the fifth card. It is an interesting exercise to come up with a simple, easy-to-remember strategy for executing this trick, but right now you have another concern.

You were planning to perform this trick today, but just now you have learned that the deck has more cards than you expected. The trick may be impossible! In desperation, you have decided to cheat a little. You have $m$ distinguishable ways of marking the backs of the playing cards. You have marked the backs of all $n$ cards, allowing you to narrow down the possibilities for the $k^{th}$ card. For example, if there are $6$ cards marked with a particular method, and you see that the back of the $k^{th}$ card is marked with that method, you know it must be one of those $6$ cards.

Determine the probability that you will successfully guess the $k^{th}$ card, assuming you and the assistant execute an optimal (but likely very complicated!) strategy.

## 输入格式
The input contains one line with several integers. The first integer gives $k$ ($2 \leq k \leq 10$), the number of cards that will be selected. The second integer gives $m$ ($1 \leq m \leq 10$), the number of ways of marking the cards. The line is completed by $m$ positive integers, giving the number of cards marked with each distinct method. The sum of these $m$ integers is $n$ ($k \leq n \leq 10^9$), which is the size of the deck.

## 输出格式
Output the highest possible probability of guessing the $k^{th}$ card correctly, accurate up to an absolute error of $10^{-9}$.

## 题目大意
#### 简要题意
两个人 $A, B$ 玩一个游戏。规则如下 :

$A$ 有 $n$ 张互不相同的牌. 它们的**背面**有 $m$ 种不同的样式, 第 $i$ 种牌有 $a_i$ 张. 二人都对这套牌非常了解. 保证 $\sum\limits^{m}_{i=1}{a_i} = n$.

$B$ 在 $A$ 不在场的情况下从中随机抽出 $k$ 张, 然后选择一张牌倒置在桌面上. 然后 $B$ 可以以任意顺序重新排列其他牌并在桌面上依次排开, 并将倒置的牌放在序列的末尾. $A$ 和 $B$ 可以在游戏之前约定通过其他牌的排列顺序传递的信息.

随后 $A$ 需要根据桌面上牌的排列和倒置牌的背面说出倒置的牌具体是哪一张. 双方的目标都是使 $A$ 说出正确的牌。

现在给定 $m, a_i$ 和 $k$, 求二人均采取最佳策略的情况下, $A$ 的成功率是多少.

#### 输入格式
输入仅一行, 首先是两个整数 $k, m$, 然后是 $m$ 个整数 $a_i$.

#### 输出格式
一行, 一个实数, 表示答案. 答案与标准答案的差不超过 $10^{-9}$ 即判为正确.

```input1
4 1 28

```

```output1
0.960000000000

```

```input2
3 3 5 12 3

```

```output2
0.854385964912

```

