## Description

<div><p>Dima loves watching soccer. In such a game, the score on the scoreboard is represented as $x$ : $y$, where $x$ is the number of goals of the first team, and $y$ is the number of goals of the second team. At any given time, only one team can score a goal, so the score $x$ : $y$ can change to either $(x + 1)$ : $y$, or $x$ : $(y + 1)$.</p><p>While watching a soccer game, Dima was distracted by very important matters, and after some time, he returned to watching the game. Dima remembers the score right before he was distracted, and the score right after he returned. Given these two scores, he wonders the following question. Is it possible that, <span class="tex-font-style-bf">while Dima was not watching the game</span>, the teams never had an equal score?</p><p>It is guaranteed that at neither of the two time points Dima remembers the teams had equal scores. However, it is possible that the score did not change during his absence.</p><p>Help Dima and answer the question!</p></div><div class="input-specification"><p>Each test consists of several test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains two integers $x_{1}, y_{1}$ ($0 \le x_{1}, y_{1} \le 10^{9}$, $x_{1} \neq y_{1}$)&nbsp;！ the score before Dima was distracted.</p><p>The second line of each test case contains two integers $x_{2}, y_{2}$ ($x_{1} \le x_{2} \le 10^{9}$, $y_{1} \le y_{2} \le 10^{9}$, $x_{2} \neq y_{2}$)&nbsp;！ the score when Dima returned.</p></div><div class="output-specification"><p>For each test case, output "<span class="tex-font-style-tt">YES</span>" without quotes if it is possible, that the teams never had a tie while Dima was away, otherwise output "<span class="tex-font-style-tt">NO</span>" without quotes.</p><p>You can output each letter in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p></div>

## Input

<p>Each test consists of several test cases. The first line contains an integer $t$ ($1 \le t \le 10^{4}$)&nbsp;！ the number of test cases. Then follows the description of the test cases.</p><p>The first line of each test case contains two integers $x_{1}, y_{1}$ ($0 \le x_{1}, y_{1} \le 10^{9}$, $x_{1} \neq y_{1}$)&nbsp;！ the score before Dima was distracted.</p><p>The second line of each test case contains two integers $x_{2}, y_{2}$ ($x_{1} \le x_{2} \le 10^{9}$, $y_{1} \le y_{2} \le 10^{9}$, $x_{2} \neq y_{2}$)&nbsp;！ the score when Dima returned.</p>

## Output

<p>For each test case, output "<span class="tex-font-style-tt">YES</span>" without quotes if it is possible, that the teams never had a tie while Dima was away, otherwise output "<span class="tex-font-style-tt">NO</span>" without quotes.</p><p>You can output each letter in any case (for example, the strings "<span class="tex-font-style-tt">yEs</span>", "<span class="tex-font-style-tt">yes</span>", "<span class="tex-font-style-tt">Yes</span>", and "<span class="tex-font-style-tt">YES</span>" will be recognized as a positive answer).</p>





```input1|2,3,6,7,10,11
6
1 0
5 0
1 2
3 2
1 2
4 5
1 2
4 3
1 2
1 2
998244353 0
1000000000 999999999
```




```output1
YES
NO
YES
NO
YES
YES
```



## Note

<p>In the first test case, the score before Dima left was $1$ : $0$. When he leaves, the first team scores several goals in a row until the score becomes $5$ : $0$, so the answer is <span class="tex-font-style-tt">YES</span>.</p><p>In the second test case, the score could only change as follows:</p><ul> <li> $1$ : $2$ </li><li> $2$ : $2$ </li><li> $3$ : $2$ </li></ul><p>In this scenario, there is a moment when the teams have an equal score, so the answer is <span class="tex-font-style-tt">NO</span>.</p><p>In the third test case, one of the possible developments is:</p><ul> <li> $1$ : $2$ </li><li> $1$ : $3$ </li><li> $2$ : $3$ </li><li> $2$ : $4$ </li><li> $2$ : $5$ </li><li> $3$ : $5$ </li><li> $4$ : $5$ </li></ul><p>In this scenario, there was no time when the score was equal, so the answer is <span class="tex-font-style-tt">YES</span>.</p>
