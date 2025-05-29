## Description

<div><p>Bodya and Sasha found a permutation $p_1,\dots,p_n$ and an array $a_1,\dots,a_n$. They decided to play a well-known "Permutation game".</p><p>A permutation of length $n$ is an array consisting of $n$ distinct integers from $1$ to $n$ in arbitrary order. For example, $[2,3,1,5,4]$ is a permutation, but $[1,2,2]$ is not a permutation ($2$ appears twice in the array), and $[1,3,4]$ is also not a permutation ($n=3$ but there is $4$ in the array).</p><p>Both of them chose a starting position in the permutation.</p><p>The game lasts $k$ turns. The players make moves simultaneously. On each turn, two things happen to each player: </p><ul> <li> If the current position of the player is $x$, his score increases by $a_x$. </li><li> Then the player either <span class="tex-font-style-bf">stays</span> at his current position $x$ or <span class="tex-font-style-bf">moves</span> from $x$ to $p_x$. </li></ul> The winner of the game is the player with the higher score after exactly $k$ turns.<p>Knowing Bodya's starting position $P_B$ and Sasha's starting position $P_S$, determine who wins the game if both players are trying to win.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;！ the number of testcases.</p><p>The first line of each testcase contains integers $n$, $k$, $P_B$, $P_S$ ($1\le P_B,P_S\le n\le 2\cdot 10^5$, $1\le k\le 10^9$)&nbsp;！ length of the permutation, duration of the game, starting positions respectively.</p><p>The next line contains $n$ integers $p_1,\dots,p_n$ ($1 \le p_i \le n$)&nbsp;！ elements of the permutation $p$.</p><p>The next line contains $n$ integers $a_1,\dots,a_n$ ($1\le a_i\le 10^9$)&nbsp;！ elements of array $a$.</p><p>It is guaranteed that the sum of values of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p></div><div class="output-specification"><p>For each testcase output: </p><ul> <li> "<span class="tex-font-style-tt">Bodya</span>" if Bodya wins the game. </li><li> "<span class="tex-font-style-tt">Sasha</span>" if Sasha wins the game. </li><li> "<span class="tex-font-style-tt">Draw</span>" if the players have the same score. </li></ul></div>

## Input

<p>The first line contains a single integer $t$ ($1\le t\le 10^4$)&nbsp;！ the number of testcases.</p><p>The first line of each testcase contains integers $n$, $k$, $P_B$, $P_S$ ($1\le P_B,P_S\le n\le 2\cdot 10^5$, $1\le k\le 10^9$)&nbsp;！ length of the permutation, duration of the game, starting positions respectively.</p><p>The next line contains $n$ integers $p_1,\dots,p_n$ ($1 \le p_i \le n$)&nbsp;！ elements of the permutation $p$.</p><p>The next line contains $n$ integers $a_1,\dots,a_n$ ($1\le a_i\le 10^9$)&nbsp;！ elements of array $a$.</p><p>It is guaranteed that the sum of values of $n$ over all test cases does not exceed $2 \cdot 10^5$.</p>

## Output

<p>For each testcase output: </p><ul> <li> "<span class="tex-font-style-tt">Bodya</span>" if Bodya wins the game. </li><li> "<span class="tex-font-style-tt">Sasha</span>" if Sasha wins the game. </li><li> "<span class="tex-font-style-tt">Draw</span>" if the players have the same score. </li></ul>





```input1|2,3,4,8,9,10,14,15,16,20,21,22,26,27,28
10
4 2 3 2
4 1 2 3
7 2 5 6
10 8 2 10
3 1 4 5 2 7 8 10 6 9
5 10 5 1 3 7 10 15 4 3
2 1000000000 1 2
1 2
4 4
8 10 4 1
5 1 4 3 2 8 6 7
1 1 2 1 2 100 101 102
5 1 2 5
1 2 4 5 3
4 6 9 4 2
4 2 3 1
4 1 3 2
6 8 5 3
6 9 5 4
6 1 3 5 2 4
6 9 8 9 5 10
4 8 4 2
2 3 4 1
5 2 8 7
4 2 3 1
4 1 3 2
6 8 5 3
2 1000000000 1 2
1 2
1000000000 2
```




```output1
Bodya
Sasha
Draw
Draw
Bodya
Sasha
Sasha
Sasha
Sasha
Bodya
```



## Note

<p>Below you can find the explanation for the first testcase, where the game consists of $k=2$ turns.</p><center> <table class="tex-tabular"><tbody><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Turn</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Bodya's position</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Bodya's score</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Bodya's move</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Sasha's position</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Sasha's score</span></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"><span class="tex-font-style-bf">Sasha's move</span></td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">first</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0 + a_3 = 0 + 5 = 5$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">stays on the same position</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$0 + a_2 = 0 + 2 = 2$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">moves to $p_2=1$</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">second</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$5 + a_3 = 5 + 5 = 10$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">stays on the same position</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$2 + a_1 = 2 + 7 = 9$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">stays on the same position</td></tr><tr><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">final results</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$3$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$10$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"></td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$1$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom">$9$</td><td class="tex-tabular-border-left tex-tabular-text-align-center tex-tabular-border-right tex-tabular-border-top tex-tabular-border-bottom"></td></tr></tbody></table> </center><p>As we may see, Bodya's score is greater, so he wins the game. It can be shown that Bodya always can win this game.</p>
