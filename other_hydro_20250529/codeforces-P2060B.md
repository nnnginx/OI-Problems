## Description

<div><p>Farmer John's $n$ cows are playing a card game! Farmer John has a deck of $n \cdot m$ cards numbered from $0$ to $n \cdot m-1$. He distributes $m$ cards to each of his $n$ cows.</p><p>Farmer John wants the game to be fair, so each cow should only be able to play $1$ card per round. He decides to determine a <span class="tex-font-style-it">turn order</span>, determined by a permutation$^{\text{∗}}$ $p$ of length $n$, such that the $p_i$'th cow will be the $i$'th cow to place a card on top of the center pile in a round.</p><p>In other words, the following events happen in order in each round: </p><ul> <li> The $p_1$'th cow places any card from their deck on top of the center pile. </li><li> The $p_2$'th cow places any card from their deck on top of the center pile. </li><li> ... </li><li> The $p_n$'th cow places any card from their deck on top of the center pile. </li></ul><p>There is a catch. Initially, the center pile contains a card numbered $-1$. In order to place a card, the number of the card must be greater than the number of the card on top of the center pile. Then, the newly placed card becomes the top card of the center pile. If a cow cannot place any card in their deck, the game is considered to be lost.</p><p>Farmer John wonders: does there exist $p$ such that it is possible for all of his cows to empty their deck after playing all $m$ rounds of the game? If so, output any valid $p$. Otherwise, output $-1$.</p><div class="statement-footnote"><p>$^{\text{∗}}$A permutation of length $n$ contains each integer from $1$ to $n$ exactly once</p></div></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 400$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n \cdot m \leq 2\,000$) — the number of cows and the number of cards each cow receives.</p><p>The following $n$ lines contain $m$ integers each&nbsp;– the cards received by each cow. It is guaranteed all given numbers (across all $n$ lines) are distinct and in the range from $0$ to $n \cdot m - 1$, inclusive.</p><p>It is guaranteed the sum of $n \cdot m$ over all test cases does not exceed $2\,000$.</p></div><div class="output-specification"><p>For each test case, output the following on a new line:</p><ul> <li> If $p$ exists, output $n$ space-separated integers $p_1, p_2, \ldots, p_n$. </li><li> Otherwise, output $-1$. </li></ul></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 400$) — the number of test cases.</p><p>The first line of each test case contains two integers $n$ and $m$ ($1 \leq n \cdot m \leq 2\,000$) — the number of cows and the number of cards each cow receives.</p><p>The following $n$ lines contain $m$ integers each&nbsp;– the cards received by each cow. It is guaranteed all given numbers (across all $n$ lines) are distinct and in the range from $0$ to $n \cdot m - 1$, inclusive.</p><p>It is guaranteed the sum of $n \cdot m$ over all test cases does not exceed $2\,000$.</p>

## Output

<p>For each test case, output the following on a new line:</p><ul> <li> If $p$ exists, output $n$ space-separated integers $p_1, p_2, \ldots, p_n$. </li><li> Otherwise, output $-1$. </li></ul>





```input1|2,3,4,7,8,9
4
2 3
0 4 2
1 5 3
1 1
0
2 2
1 2
0 3
4 1
1
2
0
3
```




```output1
1 2
1
-1
3 1 2 4
```



## Note

<p>In the first test case, one turn order that allows all cards to be played is by having the first cow go before the second cow. The cards played will be $0\rightarrow1\rightarrow2\rightarrow3\rightarrow4\rightarrow5$.</p><p>In the second test case, there is only one cow, so having the cow play all of her cards in increasing order will empty the deck.</p><p>In the third test case, it can be shown there is no valid turn order that allows all cards to be played.</p>
