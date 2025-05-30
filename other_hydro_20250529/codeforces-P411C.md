## Description

<div><p>Kicker (table football) is a board game based on football, in which players control the footballers' figures mounted on rods by using bars to get the ball into the opponent's goal. When playing two on two, one player of each team controls the goalkeeper and the full-backs (plays defence), the other player controls the half-backs and forwards (plays attack).</p><p>Two teams of company Q decided to battle each other. Let's enumerate players from both teams by integers from <span class="tex-span">1</span> to <span class="tex-span">4</span>. The first and second player play in the first team, the third and the fourth one play in the second team. For each of the four players we know their game skills in defence and attack. The defence skill of the <span class="tex-span"><i>i</i></span>-th player is <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, the attack skill is <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Before the game, the teams determine how they will play. First the players of the first team decide who will play in the attack, and who will play in the defence. Then the second team players do the same, based on the choice of their opponents.</p><p>We will define a team's defence as the defence skill of player of the team who plays defence. Similarly, a team's attack is the attack skill of the player of the team who plays attack. We assume that one team is guaranteed to beat the other one, if its defence is strictly greater than the opponent's attack and its attack is strictly greater than the opponent's defence.</p><p>The teams of company Q know each other's strengths and therefore arrange their teams optimally. Identify the team that is guaranteed to win (if both teams act optimally) or tell that there is no such team.</p></div><div class="input-specification"><p>The input contain the players' description in four lines. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the defence and the attack skill of the <span class="tex-span"><i>i</i></span>-th player, correspondingly.</p></div><div class="output-specification"><p>If the first team can win, print phrase "<span class="tex-font-style-tt">Team 1</span>" (without the quotes), if the second team can win, print phrase "<span class="tex-font-style-tt">Team 2</span>" (without the quotes). If no of the teams can definitely win, print "<span class="tex-font-style-tt">Draw</span>" (without the quotes).</p></div>


## Input

<p>The input contain the players' description in four lines. The <span class="tex-span"><i>i</i></span>-th line contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span> — the defence and the attack skill of the <span class="tex-span"><i>i</i></span>-th player, correspondingly.</p>


## Output

<p>If the first team can win, print phrase "<span class="tex-font-style-tt">Team 1</span>" (without the quotes), if the second team can win, print phrase "<span class="tex-font-style-tt">Team 2</span>" (without the quotes). If no of the teams can definitely win, print "<span class="tex-font-style-tt">Draw</span>" (without the quotes).</p>


## Samples

```input1
1 100
100 1
99 99
99 99

```

```output1
Team 1

```






```input2
1 1
2 2
3 3
2 2

```

```output2
Team 2

```






```input3
3 3
2 2
1 1
2 2

```

```output3
Draw

```




## Note

<p>Let consider the first test sample. The first team can definitely win if it will choose the following arrangement: the first player plays attack, the second player plays defence.</p><p>Consider the second sample. The order of the choosing roles for players makes sense in this sample. As the members of the first team choose first, the members of the second team can beat them (because they know the exact defence value and attack value of the first team).</p>

