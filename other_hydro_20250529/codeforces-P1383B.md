## Description

<div><p>Koa the Koala and her best friend want to play a game.</p><p>The game starts with an array $a$ of length $n$ consisting of non-negative integers. Koa and her best friend move in turns and each have initially a score equal to $0$. Koa starts.</p><p>Let's describe a move in the game:</p><ul> <li> During his move, a player chooses any element of the array and removes it from this array, xor-ing it with the current score of the player.<p> More formally: if the current score of the player is $x$ and the chosen element is $y$, his new score will be $x \oplus y$. Here $\oplus$ denotes <a href="https://en.wikipedia.org/wiki/Bitwise_operation#XOR">bitwise XOR operation</a>.</p><p> Note that after a move element $y$ is removed from $a$.</p><p> </p></li><li> The game ends when the array is empty. </li></ul><p>At the end of the game the winner is the player with the maximum score. If both players have the same score then it's a draw.</p><p>If both players play optimally find out whether Koa will win, lose or draw the game.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains the integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the length of $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;！ elements of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p></div><div class="output-specification"><p>For each test case print:</p><ul> <li> <span class="tex-font-style-tt">WIN</span> if Koa will win the game. </li><li> <span class="tex-font-style-tt">LOSE</span> if Koa will lose the game. </li><li> <span class="tex-font-style-tt">DRAW</span> if the game ends in a draw. </li></ul></div>

## Input

<p>Each test contains multiple test cases. The first line contains $t$ ($1 \le t \le 10^4$)&nbsp;！ the number of test cases. Description of the test cases follows.</p><p>The first line of each test case contains the integer $n$ ($1 \le n \le 10^5$)&nbsp;！ the length of $a$.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;！ elements of $a$.</p><p>It is guaranteed that the sum of $n$ over all test cases does not exceed $10^5$.</p>

## Output

<p>For each test case print:</p><ul> <li> <span class="tex-font-style-tt">WIN</span> if Koa will win the game. </li><li> <span class="tex-font-style-tt">LOSE</span> if Koa will lose the game. </li><li> <span class="tex-font-style-tt">DRAW</span> if the game ends in a draw. </li></ul>

## Samples

```input1
3
3
1 2 2
3
2 2 3
5
0 0 0 2 2
```

```output1
WIN
LOSE
DRAW
```






```input2
4
5
4 1 5 1 3
4
1 0 1 6
1
0
2
5 4
```

```output2
WIN
WIN
DRAW
WIN
```




## Note

<p>In testcase $1$ of the first sample we have:</p><p>$a = [1, 2, 2]$. Here Koa chooses $1$, other player has to choose $2$, Koa chooses another $2$. Score for Koa is $1 \oplus 2 = 3$ and score for other player is $2$ so Koa wins.</p>
