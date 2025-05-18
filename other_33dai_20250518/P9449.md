## 题目描述
The Internet can be so fickle. You work for a small ad agency, Mimi's Mammoth Memes. Your ad campaigns are very cheap, and rely on the hope of producing the next hit viral meme. Unfortunately, the last four hundred or so memes have failed to take off, despite having been precisely engineered to appeal to every single person on Earth. You're not sure what exactly went wrong, but you've decided to try a new approach: crowd sourcing!

According to your scientific meme theory, all memes can be rated from $-\infty$ to $\infty$ on two scales: xanthochromism, and yellowishness, also known as ($x$, $y$) values. Obviously (you think), the best memes are memorable for being particularly xanthochromic, yellowish, unxanthochromic, or unyellowish. You feel that the "quality" of any meme is directly measurable as its squared Euclidean distance ($x^2 + y^2$) from the Base Meme ($0$, $0$), otherwise known as All Your Base.

To produce the ultimate viral meme, you'll be taking your company's last few failed memes and throwing them into a tournament, decided by online voting. The tournament can be represented as a rooted tree. Input memes come in at the leaves, and at each internal node, a vote will be held among its $k$ child memes ($x_1$, $y_1$), $\ldots$, ($x_k$, $y_k$). After the vote, all the memes will be horrifically mangled and merged into a brand new meme, specifically calculated to emphasize the winner and de-emphasize all the losers: the resultant $x$ value will be $$ \sum_{i=1}^{k} w_i \cdot x_i, $$ where $w_i$ is $1$ if the $i^{th}$ child won, and $-1$ otherwise. The $y$ value is computed similarly. This new meme will move on to the next vote in the tournament $-$ or, if there is no parent, it will be declared the champion and the ultimate meme!

You already have the structure of the tournament planned out, including all the input memes and the internal voting nodes. What is the largest possible quality for any meme that the tournament could produce?

## 输入格式
The first line of input contains an integer $n$ ($1 \leq n \leq 10^4$), giving the total number of nodes in the tournament tree. The next $n$ lines each describe a single tree node indexed from $1$ to $n$. The line for node $i$ starts with an integer $k_i$ ($0 \leq k_i \leq 100$), the number of children of that node. If $k_i$ is $0$, then node $i$ is an input meme and there will be two more integers $x_i$ and $y_i$ ($-10^3 \leq x_i, yi \leq 10^3$) describing it. If $k_i &gt; 0$, then $k_i$ different integers $j$ ($i &lt; j \leq n$) will follow, giving the indices of the $k_i$ nodes entering this voting step.

All input memes will eventually be merged into the final output meme at node $1$. The complete tree will have a height of no more than $10$.

## 输出格式
Output the largest possible quality for the champion meme at node $1$.

## 题目大意
众所周知，互联网的走红规律总是难以捉摸。你就职于一家名为 Mimi's Mammoth Memes 的小型广告公司。你们的广告策略非常经济实惠，全靠碰运气，使得下一个爆红的病毒式梗图诞生。然而，尽管你们精心设计过，最近的四百多个梗图却无一火爆。你对问题的具体原因并不十分清楚，但决定尝试一种全新的方法：众包创意！

根据你的梗图科学理论，所有梗图都可以在两个维度上被评分，分别是鲜艳度和泛黄程度，简称为 $(x, y)$ 值。显然（你这样认为），最出众的梗图要么特别鲜艳，要么特别不鲜艳，要么特别泛黄，要么特别不泛黄。你认为，一个梗图的“质量”可以直接通过它和基础梗图 $(0, 0)$ 的欧几里得距离平方来衡量，即计算 $(x^2 + y^2)$。

为了创造出终极病毒式梗图，你将把公司最近几个不成功的梗图放入一个通过在线投票来决胜负的锦标赛中。这个锦标赛可以用一棵有根树来表示。输入梗图位于叶子节点，在每个内部节点，针对其 $k$ 个子梗图 $(x_1, y_1),\cdots, (x_k, y_k)$ 进行投票。投票后，梗图将经历恐怖的扭曲并合并成一个新梗图，特别突出了胜者并削弱了所有的败者：得到的 $x$ 值为 

$$ \sum_{i=1}^{k} w_i \cdot x_i, $$ 

其中当第 $i$ 个梗图获胜时，$w_i$ 为 $1$，否则为 $-1$。$y$ 值的计算方式相同。该新梗图将进入锦标赛下一轮的投票——如果它没有父节点，则会被宣布为冠军，也就是最终的完美梗图！

你已经设计好了锦标赛的结构，包括所有输入的梗图和内部的投票节点。那么，该锦标赛可能产生的梗图质量的最大值是多少？

## 输入格式

输入的第一行包含一个整数 $n$ ($1 \leq n \leq 10^4$)，表示锦标赛树中的节点总数。接下来的 $n$ 行，每行描述一个编号从 $1$ 到 $n$ 的节点。对于节点 $i$，这一行先出现一个整数 $k_i$ ($0 \leq k_i \leq 100$)，表示该节点的子节点数。如果 $k_i$ 为 0，则表明节点 $i$ 是一个输入梗图，并包含两个额外整数 $x_i$ 和 $y_i$ ($-10^3 \leq x_i, y_i \leq 10^3$)，描述该梗图的特征值。如果 $k_i > 0$，则接下来会出现 $k_i$ 个不同的整数 $j$ ($i < j \leq n$)，表示参与这一投票步骤的节点索引。

所有输入的梗图将最终被合并为节点 $1$ 中的最终输出梗图。整个树的高度不会超过 $10$。

## 输出格式

输出节点 $1$ 的冠军梗图的最大可能质量。


```input1
4
3 2 3 4
0 10 1
0 3 6
0 2 7

```

```output1
169
```

```input2
8
3 4 2 5
2 3 8
0 -3 9
0 -5 -7
2 6 7
0 1 4
0 -3 -1
0 1 4

```

```output2
314
```

