## Description

<div><p>Let's introduce a two-player game, table tennis, where a winner is always decided and draws are impossible.</p><p>Three players, Sosai, Fofo, and Hohai, want to spend the rest of their lives playing table tennis. They decided to play forever in the following way:</p><ul> <li> In each match, two players compete while the third spectates.<p> </p></li><li> To ensure fairness, no player can play three times in a row. The player who plays twice in a row must sit out as a spectator in the next match, which will be played by the other two players. Otherwise, the winner and the spectator will play in the next match, while the loser will spectate. </li></ul><p>Now, the players, fully immersed in this infinite loop of matches, have tasked you with solving the following problem:</p><p>Given an integer $k$, determine whether the spectator of the first match can be the spectator in the $k$-th match.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). The description of the test cases follows. </p><p>The only line of each test case contains one integer $k$ ($1 \le k \le 10^9$).</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">"YES"</span> (without quotes) if the spectator of the first match can be the spectator of the $k$-th match, and <span class="tex-font-style-tt">"NO"</span> (without quotes) otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings <span class="tex-font-style-tt">"yEs"</span>, <span class="tex-font-style-tt">"yes"</span>, <span class="tex-font-style-tt">"Yes"</span>, and <span class="tex-font-style-tt">"YES"</span> will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 1000$). The description of the test cases follows. </p><p>The only line of each test case contains one integer $k$ ($1 \le k \le 10^9$).</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">"YES"</span> (without quotes) if the spectator of the first match can be the spectator of the $k$-th match, and <span class="tex-font-style-tt">"NO"</span> (without quotes) otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings <span class="tex-font-style-tt">"yEs"</span>, <span class="tex-font-style-tt">"yes"</span>, <span class="tex-font-style-tt">"Yes"</span>, and <span class="tex-font-style-tt">"YES"</span> will be recognized as positive responses.</p>





```input1|2,4
4
1
2
333
1000000000
```




```output1
YES
NO
NO
YES
```



## Note

<p>In the first test case, the spectator of the first match is already a spectator in the $1$st match.</p><p>In the second test case, the spectator of the first match will play in the $2$nd match regardless of the result of the first match.</p>
