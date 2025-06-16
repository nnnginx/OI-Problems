## Description

<div><p><span class="tex-font-style-it">Something you may not know about Mouf is that he is a big fan of the Yu-Gi-Oh! card game. He loves to duel with anyone he meets. To gather all fans who love to play as well, he decided to organize a big Yu-Gi-Oh! tournament and invited $n$ players.</span></p><p>Mouf arranged the $n$ players in a line, numbered from $1$ to $n$. They then held $n - 1$ consecutive duels: for each $i$ from $1$ to $n - 1$, player $i$ faced player $i + 1$, producing one winner and one loser per match. Afterward, each player reports a value $a_i(0 \le a_i \le 1)$:</p><ul> <li> $0$ indicating they won no duels; </li><li> $1$ indicating they won at least one duel. </li></ul><p>Since some may lie about their results (e.g., reporting a $1$ instead of a $0$, or vice versa) to influence prize outcomes, Mouf will cancel the tournament if he can prove any report to be false.</p><p>Given the array $a$, determine whether at least one player must be lying.</p></div><div class="input-specification"><p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains one integer $n$ ($2 \le n \le 100$)&nbsp;！ the number of players in the tournament.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 1$)&nbsp;！ denoting the report of the $i$-th player.</p></div><div class="output-specification"><p>For each test case, print <span class="tex-font-style-tt">"YES"</span> (without quotes) if there is at least one liar among the players, and <span class="tex-font-style-tt">"NO"</span> (without quotes) otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings <span class="tex-font-style-tt">"yEs"</span>, <span class="tex-font-style-tt">"yes"</span>, <span class="tex-font-style-tt">"Yes"</span>, and <span class="tex-font-style-tt">"YES"</span> will be recognized as positive responses.</p></div>

## Input

<p>Each test contains multiple test cases. The first line contains the number of test cases $t$ ($1 \le t \le 100$). The description of the test cases follows. </p><p>The first line of each test case contains one integer $n$ ($2 \le n \le 100$)&nbsp;！ the number of players in the tournament.</p><p>The second line of each test case contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 1$)&nbsp;！ denoting the report of the $i$-th player.</p>

## Output

<p>For each test case, print <span class="tex-font-style-tt">"YES"</span> (without quotes) if there is at least one liar among the players, and <span class="tex-font-style-tt">"NO"</span> (without quotes) otherwise.</p><p>You can output the answer in any case (upper or lower). For example, the strings <span class="tex-font-style-tt">"yEs"</span>, <span class="tex-font-style-tt">"yes"</span>, <span class="tex-font-style-tt">"Yes"</span>, and <span class="tex-font-style-tt">"YES"</span> will be recognized as positive responses.</p>





```input1|2,3,6,7,10,11
6
3
0 1 0
2
0 0
2
1 1
4
0 1 1 1
4
1 0 0 1
7
0 1 0 1 0 1 0
```




```output1
NO
YES
YES
NO
YES
NO
```



## Note

<p>In the first test case, it is consistent if player $2$ defeats both players $1$ and $3$, so nobody's report is necessarily false.</p><p>In the second test case, in the only match between players $1$ and $2$, one must win ！ but both claimed zero wins, so someone must be lying.</p><p>In the third test case, the tournament consists of exactly one duel between players $1$ and $2$ ！ but it's impossible for both to win, concluding that at least one report is false.</p><p>In the fourth test case, a possible scenario is that player $2$ won against player $1$, then $3$ won against $2$, and then $4$ won against $3$. All reports align, so there is no evidence that someone lied.</p>
