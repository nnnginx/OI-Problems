## Description

<div><p><span class="tex-font-style-it">This is an interactive problem.</span></p><p>John and his imaginary friend play a game. There are $n$ lamps arranged in a circle. Lamps are numbered $1$ through $n$ in clockwise order, that is, lamps $i$ and $i + 1$ are adjacent for any $i = 1, \ldots, n - 1$, and also lamps $n$ and $1$ are adjacent. Initially all lamps are turned off.</p><p>John and his friend take turns, with John moving first. On his turn John can choose to terminate the game, or to make a move. To make a move, John can choose any positive number $k$ and turn any $k$ lamps of his choosing on. In response to this move, John's friend will choose $k$ <span class="tex-font-style-bf">consecutive</span> lamps and turn all of them off (the lamps in the range that were off before this move stay off). Note that the value of $k$ is the same as John's number on his last move. For example, if $n = 5$ and John have just turned three lamps on, John's friend may choose to turn off lamps $1, 2, 3$, or $2, 3, 4$, or $3, 4, 5$, or $4, 5, 1$, or $5, 1, 2$.</p><p>After this, John may choose to terminate or move again, and so on. However, John can not make more than $10^4$ moves.</p><p>John wants to maximize the number of lamps turned on at the end of the game, while his friend wants to minimize this number. Your task is to provide a strategy for John to achieve optimal result. Your program will play interactively for John against the jury's interactor program playing for John's friend.</p><p>Suppose there are $n$ lamps in the game. Let $R(n)$ be the number of turned on lamps at the end of the game if both players act optimally. Your program has to terminate the game with at least $R(n)$ turned on lamps within $10^4$ moves. Refer to Interaction section below for interaction details.</p><p>For technical reasons <span class="tex-font-style-bf">hacks for this problem are disabled.</span></p></div><div><h2>Interaction</h2><p>Initially your program will be fed a single integer $n$ ($1 \leq n \leq 1000$)&nbsp;�� the number of lamps in the game. Then the interactor will wait for your actions.</p><p>To make a move, print a line starting with an integer $k$ ($1 \leq k \leq n$), followed by $k$ <span class="tex-font-style-bf">distinct</span> integers $l_1, \ldots, l_k$ ($1 \leq l_i \leq n$)&nbsp;�� indices of lamps you want to turn on. The indices may be printed in any order. It is allowed to try to turn on a lamp that is already on (although this will have no effect).</p><p>If your move was invalid for any reason, or if you have made more than $10^4$ moves, the interactor will reply with a line containing a single integer $-1$. Otherwise, the reply will be a line containing a single integer $x$ ($1 \leq x \leq n)$, meaning that the response was to turn off $k$ consecutive lamps starting from $x$ in clockwise order.</p><p>To terminate the game instead of making a move, print a line containing a single integer $0$. The test will be passed if at this point there are at least $R(n)$ lamps turned on (note that neither $R(n)$, nor the verdict received are not communicated to your program in any way). This action does not count towards the number of moves (that is, it is legal to terminate the game after exactly $10^4$ moves).</p><p>To receive the correct verdict, your program should terminate immediately after printing $0$, or after receiving $-1$ as a response.</p><p>Don't forget to flush your output after every action.</p></div>

## Samples

```input1
3
```

```output1
0
```






```input2
4

1
```

```output2
2 1 3

0
```




## Note

<p>When $n = 3$, any John's move can be reversed, thus $R(3) = 0$, and terminating the game immediately is correct.</p><p>$R(4) = 1$, and one strategy to achieve this result is shown in the second sample case.</p><p>Blank lines in sample interactions are for clarity and should not be printed.</p>
