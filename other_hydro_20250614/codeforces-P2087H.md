## Description

<div><p>Let's recall the rules of the game "Nim". The game is played by two players who take turns. They have a certain number of piles of stones (the piles can be of the same size or different sizes; the size is defined as the number of stones in a pile). On their turn, a player must choose any non-empty pile of stones and remove any number of stones from it (at least one). The player who cannot make a move loses.</p><p>In this problem, a modified version of the game will be used. There is a special set of numbers $S$ that prohibits certain moves. For each number $s_i$ in this set, if the current size of the pile of stones is <span class="tex-font-style-bf">strictly greater</span> than $s_i$, it cannot be made <span class="tex-font-style-bf">strictly less</span> than $s_i$ in one move. In other words, if the current size of the pile is $x$, and the player tries to make a move that results in a size of $y$, and $x &gt; s_i &gt; y$ for some number $s_i \in S$, such a move is not allowed.</p><p>Your task is as follows. Initially, the set $S$ is empty. You need to process queries of three types:</p><ul> <li> add a certain number $s_i$ to the set; </li><li> remove a certain number $s_i$ from the set; </li><li> determine who will win if this modified version of Nim is played with piles of stones of sizes $a_1, a_2, \dots, a_k$. Assume that both players play optimally. </li></ul></div><div class="input-specification"><p>The first line contains a single integer $q$ ($1 \le q \le 3 \cdot 10^5$) ！ the number of queries.</p><p>Each query is given in one line in one of the following formats:</p><ul> <li> $1$ $s_i$ ($1 \le s_i \le 3 \cdot 10^5$) ！ if the number $s_i$ is in the set $S$, remove it; otherwise, add it to $S$; </li><li> $2$ $k_i$ $a_{i,1}$ $a_{i,2}$ ... $a_{i,k_i}$ ($1 \le k_i \le 3$; $1 \le a_{i,j} \le 3 \cdot 10^5$) ！ determine who will win the game if it uses $k_i$ piles of stones with sizes $a_{i,1}, a_{i,2}, \dots, a_{i,k_i}$. </li></ul></div><div class="output-specification"><p>For each query of type $2$, output <span class="tex-font-style-tt">First</span> if the player making the first move will win, or <span class="tex-font-style-tt">Second</span> if they will lose.</p></div>

## Input

<p>The first line contains a single integer $q$ ($1 \le q \le 3 \cdot 10^5$) ！ the number of queries.</p><p>Each query is given in one line in one of the following formats:</p><ul> <li> $1$ $s_i$ ($1 \le s_i \le 3 \cdot 10^5$) ！ if the number $s_i$ is in the set $S$, remove it; otherwise, add it to $S$; </li><li> $2$ $k_i$ $a_{i,1}$ $a_{i,2}$ ... $a_{i,k_i}$ ($1 \le k_i \le 3$; $1 \le a_{i,j} \le 3 \cdot 10^5$) ！ determine who will win the game if it uses $k_i$ piles of stones with sizes $a_{i,1}, a_{i,2}, \dots, a_{i,k_i}$. </li></ul>

## Output

<p>For each query of type $2$, output <span class="tex-font-style-tt">First</span> if the player making the first move will win, or <span class="tex-font-style-tt">Second</span> if they will lose.</p>





```input1|
11
2 2 1 4
1 2
2 2 1 4
2 3 3 1 4
1 3
2 3 3 1 4
2 2 1 4
1 4
2 2 1 5
1 2
2 2 1 5
```




```output1
First
Second
Second
Second
Second
First
Second
```


