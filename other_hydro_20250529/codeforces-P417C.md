## Description

<div><p>One day, at the "Russian Code Cup" event it was decided to play football as an out of competition event. All participants was divided into <span class="tex-span"><i>n</i></span> teams and played several matches, two teams could not play against each other more than once.</p><p>The appointed Judge was the most experienced member — Pavel. But since he was the wisest of all, he soon got bored of the game and fell asleep. Waking up, he discovered that the tournament is over and the teams want to know the results of all the matches.</p><p>Pavel didn't want anyone to discover about him sleeping and not keeping an eye on the results, so he decided to recover the results of all games. To do this, he asked all the teams and learned that the real winner was friendship, that is, each team beat the other teams exactly <span class="tex-span"><i>k</i></span> times. Help Pavel come up with chronology of the tournir that meets all the conditions, or otherwise report that there is no such table.</p></div><div class="input-specification"><p>The first line contains two integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1000</span>).</p></div><div class="output-specification"><p>In the first line print an integer <span class="tex-span"><i>m</i></span> — number of the played games. The following <span class="tex-span"><i>m</i></span> lines should contain the information about all the matches, one match per line. The <span class="tex-span"><i>i</i></span>-th line should contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). The numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> mean, that in the <span class="tex-span"><i>i</i></span>-th match the team with number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> won against the team with number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. You can assume, that the teams are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>If a tournir that meets the conditions of the problem does not exist, then print -1.</p></div>


## Input

<p>The first line contains two integers — <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 1000</span>).</p>


## Output

<p>In the first line print an integer <span class="tex-span"><i>m</i></span> — number of the played games. The following <span class="tex-span"><i>m</i></span> lines should contain the information about all the matches, one match per line. The <span class="tex-span"><i>i</i></span>-th line should contain two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>; <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub></span>). The numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> mean, that in the <span class="tex-span"><i>i</i></span>-th match the team with number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> won against the team with number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. You can assume, that the teams are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>.</p><p>If a tournir that meets the conditions of the problem does not exist, then print -1.</p>


## Samples

```input1
3 1

```

```output1
3
1 2
2 3
3 1

```



