## Description

<div><p>Suneet and Slavic play a card game. The rules of the game are as follows:</p><ul> <li> Each card has an integer value between $1$ and $10$. </li><li> Each player receives $2$ cards which are face-down (so a player doesn't know their cards). </li><li> The game is turn-based and consists <span class="tex-font-style-bf">exactly of two turns</span>. In a round, both players pick a <span class="tex-font-style-bf">random unflipped</span> card and flip it. The player who flipped a card with a strictly greater number wins the round. In case of equality, no one wins the round. </li><li> A player wins a game if he wins the most number of rounds (i.e. strictly greater than the other player). In case of equality, no one wins the game. </li></ul><p>Since Suneet and Slavic aren't best friends, you need to calculate the number of ways the game could happen that Suneet would end up as the winner.</p><p><span class="tex-font-style-it">For a better understanding, please check the notes section.</span></p></div><div class="input-specification"><p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;�� the number of test cases.</p><p>The first and only line of each test case contains $4$ integers $a_1$, $a_2$, $b_1$, $b_2$ ($1 \leq a_1, a_2, b_1, b_2 \leq 10$) where $a_1$ and $a_2$ represent the cards Suneet has, and $b_1$ and $b_2$ represent the cards Slavic has, respectively.</p></div><div class="output-specification"><p>For each test case, output a single integer&nbsp;�� the number of games Suneet would win considering all possible games.</p></div>

## Input

<p>The first line contains an integer $t$ ($1 \leq t \leq 10^4$)&nbsp;�� the number of test cases.</p><p>The first and only line of each test case contains $4$ integers $a_1$, $a_2$, $b_1$, $b_2$ ($1 \leq a_1, a_2, b_1, b_2 \leq 10$) where $a_1$ and $a_2$ represent the cards Suneet has, and $b_1$ and $b_2$ represent the cards Slavic has, respectively.</p>

## Output

<p>For each test case, output a single integer&nbsp;�� the number of games Suneet would win considering all possible games.</p>





```input1|2,4,6
5
3 8 2 6
1 1 1 1
10 10 2 2
1 1 10 10
3 8 7 2
```




```output1
2
0
4
0
2
```



## Note

<p>Consider the first test case when Slavic starts with the cards that have the values $2$ and $6$, and Suneet starts with cards that have the values $3$ and $8$. The game could happen in $4$ different ways:</p><ul> <li> Suneet flips $3$ and Slavic flips $2$. Suneet wins the first round. Then, Suneet flips $8$ and Slavic flips $6$. Suneet wins the second round as well. Since Suneet won $2$ rounds, he wins the game.<p> </p></li><li> Suneet flips $3$ and Slavic flips $6$. Slavic wins the first round. Then, Suneet flips $8$ and Slavic flips $2$. Suneet wins the second round. Nobody wins since both players won an equal amount of rounds.<p> </p></li><li> Suneet flips $8$ and Slavic flips $6$. Suneet wins the first round. Then, Suneet flips $3$ and Slavic flips $2$. Suneet wins the second round as well. Since Suneet won $2$ rounds, he wins the game.<p> </p></li><li> Suneet flips $8$ and Slavic flips $2$. Suneet wins the first round. Then, Suneet flips $3$ and Slavic flips $6$. Slavic wins the round. Nobody wins since both players won an equal amount of rounds. </li></ul>
