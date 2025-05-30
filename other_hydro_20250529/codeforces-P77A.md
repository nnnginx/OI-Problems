## Description

<div><p>The year of 2012 is coming...</p><p>According to an ancient choradrican legend in this very year, in 2012, Diablo and his brothers Mephisto and Baal will escape from hell, and innumerable hordes of demons will enslave the human world. But seven brave heroes have already gathered on the top of a mountain Arreat to protect us mere mortals from the effect of this terrible evil.</p><p>The seven great heroes are: amazon <span class="tex-font-style-tt">Anka</span>, barbarian <span class="tex-font-style-tt">Chapay</span>, sorceress <span class="tex-font-style-tt">Cleo</span>, druid <span class="tex-font-style-tt">Troll</span>, necromancer <span class="tex-font-style-tt">Dracul</span>, paladin <span class="tex-font-style-tt">Snowy</span> and a professional hit girl <span class="tex-font-style-tt">Hexadecimal</span>. Heroes already know how much experience will be given for each of the three megabosses: <span class="tex-span"><i>a</i></span> for Mephisto, <span class="tex-span"><i>b</i></span> for Diablo and <span class="tex-span"><i>c</i></span> for Baal.</p><p>Here's the problem: heroes are as much as seven and megabosses are only three! Then our heroes decided to split into three teams, where each team will go to destroy their own megaboss. Each team member will receive a <img align="middle" class="tex-formula" src="./25478/file/sKxPnbEO.png" style="max-width: 100.0%;max-height: 100.0%;"> of experience, rounded down, where <span class="tex-span"><i>x</i></span> will be the amount of experience for the killed megaboss and <span class="tex-span"><i>y</i></span> — the number of people in the team.</p><p>Heroes do not want to hurt each other's feelings, so they want to split into teams so that the difference between the hero who received the maximum number of experience and the hero who received the minimum number of experience were minimal. Since there can be several divisions into teams, then you need to find the one in which <span class="tex-font-style-underline">the total amount of liking in teams</span> were maximum.</p><p>It is known that some heroes like others. But if hero <span class="tex-span"><i>p</i></span> likes hero <span class="tex-span"><i>q</i></span>, this does not mean that the hero <span class="tex-span"><i>q</i></span> likes hero <span class="tex-span"><i>p</i></span>. No hero likes himself.</p><p>The total amount of liking in teams is the amount of ordered pairs <span class="tex-span">(<i>p</i>, <i>q</i>)</span>, such that heroes <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> are in the same group, and hero <span class="tex-span"><i>p</i></span> likes hero <span class="tex-span"><i>q</i></span> (but it is not important if hero <span class="tex-span"><i>q</i></span> likes hero <span class="tex-span"><i>p</i></span>). In case of heroes <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> likes each other and they are in the same group, this pair should be counted twice, as <span class="tex-span">(<i>p</i>, <i>q</i>)</span> and <span class="tex-span">(<i>q</i>, <i>p</i>)</span>.</p><p>A team can consist even of a single hero, but it is important that every megaboss was destroyed. All heroes must be involved in the campaign against evil. None of the heroes can be in more than one team.</p><p>It is guaranteed that every hero is able to destroy any megaboss alone.</p></div><div class="input-specification"><p>The first line contains a single non-negative integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 42</span>) — amount of liking between the heroes. Next <span class="tex-span"><i>n</i></span> lines describe liking in the form "<span class="tex-font-style-tt">p likes q</span>", meaning that the hero <span class="tex-font-style-tt">p</span> likes the hero <span class="tex-font-style-tt">q</span> (<span class="tex-font-style-tt">p</span> <span class="tex-span"> ≠ </span> <span class="tex-font-style-tt">q</span>). Every liking is described in the input exactly once, no hero likes himself.</p><p>In the last line are given three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 2·10<sup class="upper-index">9</sup></span>), separated by spaces: the experience for Mephisto, the experience for Diablo and experience for Baal.</p><p>In all the pretests, except for examples from the statement, the following condition is satisfied: <span class="tex-span"><i>a</i> = <i>b</i> = <i>c</i></span>.</p></div><div class="output-specification"><p>Print two integers — the minimal difference in the experience between two heroes who will receive the maximum and minimum number of experience points, and the maximal total amount of liking in teams (the number of friendships between heroes that end up in one team).</p><p><span class="tex-font-style-bf">When calculating the second answer, the team division should satisfy the difference-minimizing contraint. I.e. primary you should minimize the difference in the experience and secondary you should maximize the total amount of liking.</span></p></div>


## Input

<p>The first line contains a single non-negative integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">0 ≤ <i>n</i> ≤ 42</span>) — amount of liking between the heroes. Next <span class="tex-span"><i>n</i></span> lines describe liking in the form "<span class="tex-font-style-tt">p likes q</span>", meaning that the hero <span class="tex-font-style-tt">p</span> likes the hero <span class="tex-font-style-tt">q</span> (<span class="tex-font-style-tt">p</span> <span class="tex-span"> ≠ </span> <span class="tex-font-style-tt">q</span>). Every liking is described in the input exactly once, no hero likes himself.</p><p>In the last line are given three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ 2·10<sup class="upper-index">9</sup></span>), separated by spaces: the experience for Mephisto, the experience for Diablo and experience for Baal.</p><p>In all the pretests, except for examples from the statement, the following condition is satisfied: <span class="tex-span"><i>a</i> = <i>b</i> = <i>c</i></span>.</p>


## Output

<p>Print two integers — the minimal difference in the experience between two heroes who will receive the maximum and minimum number of experience points, and the maximal total amount of liking in teams (the number of friendships between heroes that end up in one team).</p><p><span class="tex-font-style-bf">When calculating the second answer, the team division should satisfy the difference-minimizing contraint. I.e. primary you should minimize the difference in the experience and secondary you should maximize the total amount of liking.</span></p>


## Samples

```input1
3
Troll likes Dracul
Dracul likes Anka
Snowy likes Hexadecimal
210 200 180

```

```output1
30 3

```






```input2
2
Anka likes Chapay
Chapay likes Anka
10000 50 50

```

```output2
1950 2

```




## Note

<p><span class="tex-font-style-bf">A note to first example:</span> it the first team should be <span class="tex-font-style-tt">Dracul</span>, <span class="tex-font-style-tt">Troll</span> and <span class="tex-font-style-tt">Anka</span>, in the second one <span class="tex-font-style-tt">Hexadecimal</span> and <span class="tex-font-style-tt">Snowy</span>, and in the third <span class="tex-font-style-tt">Cleo</span> и <span class="tex-font-style-tt">Chapay</span>.</p>

