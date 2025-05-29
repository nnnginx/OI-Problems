## Description

<div><p>Nene invented a new game based on an increasing sequence of integers $a_1, a_2, \ldots, a_k$.</p><p>In this game, initially $n$ players are lined up in a row. In each of the rounds of this game, the following happens:</p><ul> <li> Nene finds the $a_1$-th, $a_2$-th, $\ldots$, $a_k$-th players in a row. They are kicked out of the game simultaneously. If the $i$-th player in a row should be kicked out, but there are fewer than $i$ players in a row, they are skipped. </li></ul><p>Once no one is kicked out of the game in some round, all the players that are still in the game are declared as winners.</p><p>For example, consider the game with $a=[3, 5]$ and $n=5$ players. Let the players be named player <span class="tex-font-style-tt">A</span>, player <span class="tex-font-style-tt">B</span>, $\ldots$, player <span class="tex-font-style-tt">E</span> in the order they are lined up initially. Then, </p><ul> <li> Before the first round, players are lined up as <span class="tex-font-style-tt">ABCDE</span>. Nene finds the $3$-rd and the $5$-th players in a row. These are players <span class="tex-font-style-tt">C</span> and <span class="tex-font-style-tt">E</span>. They are kicked out in the first round. </li><li> Now players are lined up as <span class="tex-font-style-tt">ABD</span>. Nene finds the $3$-rd and the $5$-th players in a row. The $3$-rd player is player <span class="tex-font-style-tt">D</span> and there is no $5$-th player in a row. Thus, only player <span class="tex-font-style-tt">D</span> is kicked out in the second round. </li><li> In the third round, no one is kicked out of the game, so the game ends after this round. </li><li> Players <span class="tex-font-style-tt">A</span> and <span class="tex-font-style-tt">B</span> are declared as the winners. </li></ul><p>Nene has not yet decided how many people would join the game initially. Nene gave you $q$ integers $n_1, n_2, \ldots, n_q$ and you should answer the following question for each $1 \le i \le q$ <span class="tex-font-style-bf">independently</span>:</p><ul> <li> How many people would be declared as winners if there are $n_i$ players in the game initially? </li></ul></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 250$). The description of test cases follows.</p><p>The first line case contains two integers $k$ and $q$ ($1 \le k, q \le 100$)&nbsp;�� the length of the sequence $a$ and the number of values $n_i$ you should solve this problem for.</p><p>The second line contains $k$ integers $a_1,a_2,\ldots,a_k$ ($1\leq a_1&lt;a_2&lt;\ldots&lt;a_k\leq 100$)&nbsp;�� the sequence $a$.</p><p>The third line contains $q$ integers $n_1,n_2,\ldots,n_q$ ($1\leq n_i \leq 100$).</p></div><div class="output-specification"><p>For each test case, output $q$ integers: the $i$-th ($1\le i \le q$) of them should be the number of players declared as winners if initially $n_i$ players join the game.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 250$). The description of test cases follows.</p><p>The first line case contains two integers $k$ and $q$ ($1 \le k, q \le 100$)&nbsp;�� the length of the sequence $a$ and the number of values $n_i$ you should solve this problem for.</p><p>The second line contains $k$ integers $a_1,a_2,\ldots,a_k$ ($1\leq a_1&lt;a_2&lt;\ldots&lt;a_k\leq 100$)&nbsp;�� the sequence $a$.</p><p>The third line contains $q$ integers $n_1,n_2,\ldots,n_q$ ($1\leq n_i \leq 100$).</p>

## Output

<p>For each test case, output $q$ integers: the $i$-th ($1\le i \le q$) of them should be the number of players declared as winners if initially $n_i$ players join the game.</p>





```input1|2,3,4,8,9,10,14,15,16
6
2 1
3 5
5
5 3
2 4 6 7 9
1 3 5
5 4
3 4 5 6 7
1 2 3 4
2 3
69 96
1 10 100
1 1
100
50
3 3
10 20 30
1 10 100
```




```output1
2 
1 1 1 
1 2 2 2 
1 10 68 
50 
1 9 9
```



## Note

<p>The first test case was explained in the statement.</p><p>In the second test case, when $n=1$, the only player stays in the game in the first round. After that, the game ends and the only player is declared as a winner.</p>
