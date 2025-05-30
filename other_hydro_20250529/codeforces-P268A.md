## Description

<div><p>Manao works on a sports TV. He's spent much time watching the football games of some country. After a while he began to notice different patterns. For example, each team has two sets of uniforms: home uniform and guest uniform. When a team plays a game at home, the players put on the home uniform. When a team plays as a guest on somebody else's stadium, the players put on the guest uniform. The only exception to that rule is: when the home uniform color of the host team matches the guests' uniform, the host team puts on its guest uniform as well. For each team the color of the home and guest uniform is different.</p><p>There are <span class="tex-span"><i>n</i></span> teams taking part in the national championship. The championship consists of <span class="tex-span"><i>n</i>·(<i>n</i> - 1)</span> games: each team invites each other team to its stadium. At this point Manao wondered: how many times during the championship is a host team going to put on the guest uniform? Note that the order of the games does not affect this number.</p><p>You know the colors of the home and guest uniform for each team. For simplicity, the colors are numbered by integers in such a way that no two distinct colors have the same number. Help Manao find the answer to his question.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 30</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains a pair of distinct space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the colors of the <span class="tex-span"><i>i</i></span>-th team's home and guest uniforms, respectively.</p></div><div class="output-specification"><p>In a single line print the number of games where the host team is going to play in the guest uniform.</p></div>


## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 30</span>). Each of the following <span class="tex-span"><i>n</i></span> lines contains a pair of distinct space-separated integers <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>h</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the colors of the <span class="tex-span"><i>i</i></span>-th team's home and guest uniforms, respectively.</p>


## Output

<p>In a single line print the number of games where the host team is going to play in the guest uniform.</p>


## Samples

```input1
3
1 2
2 4
3 4

```

```output1
1

```






```input2
4
100 42
42 100
5 42
100 5

```

```output2
5

```






```input3
2
1 2
1 2

```

```output3
0

```




## Note

<p>In the first test case the championship consists of 6 games. The only game with the event in question is the game between teams 2 and 1 on the stadium of team 2.</p><p>In the second test sample the host team will have to wear guest uniform in the games between teams: 1 and 2, 2 and 1, 2 and 3, 3 and 4, 4 and 2 (the host team is written first).</p>

