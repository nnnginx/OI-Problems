## Description

<div><p>After a long day, Alice and Bob decided to play a little game. The game board consists of $n$ cells in a straight line, numbered from $1$ to $n$, where each cell contains a number $a_i$ between $1$ and $n$. Furthermore, no two cells contain the same number. </p><p>A token is placed in one of the cells. They take alternating turns of moving the token around the board, with Alice moving first. The current player can move from cell $i$ to cell $j$ only if the following two conditions are satisfied: </p><ul> <li> the number in the new cell $j$ must be strictly larger than the number in the old cell $i$ (i.e. $a_j &gt; a_i$), and </li><li> the distance that the token travels during this turn must be a multiple of the number in the old cell (i.e. $|i-j|\bmod a_i = 0$). </li></ul><p>Whoever is unable to make a move, loses. For each possible starting position, determine who wins if they both play optimally. It can be shown that the game is always finite, i.e. there always is a winning strategy for one of the players.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;�� the number of numbers.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$). Furthermore, there are no pair of indices $i \neq j$ such that $a_i = a_j$.</p></div><div class="output-specification"><p>Print $s$&nbsp;�� a string of $n$ characters, where the $i$-th character represents the outcome of the game if the token is initially placed in the cell $i$. If Alice wins, then $s_i$ has to be equal to "<span class="tex-font-style-tt">A</span>"; otherwise, $s_i$ has to be equal to "<span class="tex-font-style-tt">B</span>". </p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;�� the number of numbers.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le n$). Furthermore, there are no pair of indices $i \neq j$ such that $a_i = a_j$.</p>

## Output

<p>Print $s$&nbsp;�� a string of $n$ characters, where the $i$-th character represents the outcome of the game if the token is initially placed in the cell $i$. If Alice wins, then $s_i$ has to be equal to "<span class="tex-font-style-tt">A</span>"; otherwise, $s_i$ has to be equal to "<span class="tex-font-style-tt">B</span>". </p>

## Samples

```input1
8
3 6 5 4 2 7 1 8

```

```output1
BAAAABAB

```






```input2
15
3 11 2 5 10 9 7 13 15 8 4 12 6 1 14

```

```output2
ABAAAABBBAABAAB

```




## Note

<p>In the first sample, if Bob puts the token on the number (<span class="tex-font-style-bf">not position</span>): </p><ul> <li> $1$: Alice can move to any number. She can win by picking $7$, from which Bob has no move. </li><li> $2$: Alice can move to $3$ and $5$. Upon moving to $5$, Bob can win by moving to $8$. If she chooses $3$ instead, she wins, as Bob has only a move to $4$, from which Alice can move to $8$. </li><li> $3$: Alice can only move to $4$, after which Bob wins by moving to $8$. </li><li> $4$, $5$, or $6$: Alice wins by moving to $8$. </li><li> $7$, $8$: Alice has no move, and hence she loses immediately. </li></ul>
