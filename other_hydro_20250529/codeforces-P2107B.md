## Description

<div><p>Tom and Jerry found some apples in the basement. They decided to play a game to get some apples.</p><p>There are $n$ boxes, and the $i$-th box has $a_i$ apples inside. Tom and Jerry take turns picking up apples. Tom goes first. On their turn, they have to do the following:</p><ul> <li> Choose a box $i$ ($1 \le i \le n$) with a positive number of apples, i.e. $a_i &gt; 0$, and pick $1$ apple from this box. Note that this reduces $a_i$ by $1$. </li><li> If no valid box exists, the current player loses. </li><li> If <span class="tex-font-style-bf">after the move</span>, $\max(a_1, a_2, \ldots, a_n) - \min(a_1, a_2, \ldots, a_n) &gt; k$ holds, then the current player (who made the last move) also loses. </li></ul><p>If both players play optimally, predict the winner of the game.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n,k$ ($2 \le n \le 10^5,1\le k \le 10^9$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case, print "Tom" (without quotes) if Tom will win, or "Jerry" (without quotes) otherwise.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 10^4$). The description of the test cases follows. </p><p>The first line of each test case contains two integers $n,k$ ($2 \le n \le 10^5,1\le k \le 10^9$).</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($1 \le a_i \le 10^9$).</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case, print "Tom" (without quotes) if Tom will win, or "Jerry" (without quotes) otherwise.</p>





```input1|2,3,6,7
3
3 1
2 1 2
3 1
1 1 3
2 1
1 4
```




```output1
Tom
Tom
Jerry
```



## Note

<p>Note that neither player is necessarily playing an optimal strategy in the following games, just to give you an idea of how the game is going.</p><p>In the first test case of the example, one possible situation is shown as follows. </p><ul> <li> Tom takes an apple from the first box. The array $a$ becomes $[1, 1, 2]$. Tom does not lose because $\max(1, 1, 2) - \min(1, 1, 2) = 1 \le k$. </li><li> Jerry takes an apple from the first box as well. The array $a$ becomes $[0, 1, 2]$. Jerry loses because $\max(0, 1, 2) - \min(0, 1, 2) = 2 &gt; k$. </li></ul>
