## Description

<div><p>Vasya’s elder brother Petya loves playing computer games. In one of his favourite computer games Petya reached the final level where a fight with the boss take place.</p><p>While playing the game Petya found spell scrolls and now he is about to use them. Let’s describe the way fighting goes on this level:</p><p>1) The boss has two parameters: <span class="tex-span"><i>max</i></span> — the initial amount of health and <span class="tex-span"><i>reg</i></span> — regeneration rate per second.</p><p>2) Every scroll also has two parameters: <span class="tex-span"><i>pow</i><sub class="lower-index"><i>i</i></sub></span> — spell power measured in percents — the maximal amount of health counted off the initial one, which allows to use the scroll (i.e. if the boss has more than <span class="tex-span"><i>pow</i><sub class="lower-index"><i>i</i></sub></span> percent of health the scroll cannot be used); and <span class="tex-span"><i>dmg</i><sub class="lower-index"><i>i</i></sub></span> the damage per second inflicted upon the boss if the scroll is used. As soon as a scroll is used it disappears and another spell is cast upon the boss that inflicts <span class="tex-span"><i>dmg</i><sub class="lower-index"><i>i</i></sub></span> of damage per second upon him until the end of the game.</p><p>During the battle the actions per second are performed in the following order: first the boss gets the damage from all the spells cast upon him, then he regenerates <span class="tex-span"><i>reg</i></span> of health (at the same time he can’t have more than <span class="tex-span"><i>max</i></span> of health), then the player may use another scroll (no more than one per second).</p><p>The boss is considered to be defeated if at the end of a second he has nonpositive (<span class="tex-span"> ≤ 0</span>) amount of health.</p><p>Help Petya to determine whether he can win with the set of scrolls available to him and if he can, determine the minimal number of seconds he needs to do it.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>N</i></span>, <span class="tex-span"><i>max</i></span> and <span class="tex-span"><i>reg</i></span> (<span class="tex-span">1 ≤ <i>N</i>, <i>max</i>, <i>reg</i> ≤ 1000</span>) –– the amount of scrolls and the parameters of the boss. The next <span class="tex-span"><i>N</i></span> lines contain two integers <span class="tex-span"><i>pow</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>dmg</i><sub class="lower-index"><i>i</i></sub></span> each — the parameters of the <span class="tex-span"><i>i</i></span>-th scroll (<span class="tex-span">0 ≤ <i>pow</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>dmg</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>). </p></div><div class="output-specification"><p>In case Petya can’t complete this level, output in the single line <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, output on the first line <span class="tex-font-style-tt">YES</span>. On the second line output the minimal time after which the boss can be defeated and the number of used scrolls. In the next lines for each used scroll output space-separated number of seconds passed from the start of the battle to the moment the scroll was used and the number of the scroll. Scrolls are numbered starting from 1 in the input order. The first scroll is considered to be available to be used after <span class="tex-span">0</span> seconds.</p><p>Output scrolls in the order they were used. It is not allowed to use scrolls after the boss is defeated.</p></div>


## Input

<p>The first line contains three integers <span class="tex-span"><i>N</i></span>, <span class="tex-span"><i>max</i></span> and <span class="tex-span"><i>reg</i></span> (<span class="tex-span">1 ≤ <i>N</i>, <i>max</i>, <i>reg</i> ≤ 1000</span>) –– the amount of scrolls and the parameters of the boss. The next <span class="tex-span"><i>N</i></span> lines contain two integers <span class="tex-span"><i>pow</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>dmg</i><sub class="lower-index"><i>i</i></sub></span> each — the parameters of the <span class="tex-span"><i>i</i></span>-th scroll (<span class="tex-span">0 ≤ <i>pow</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>, <span class="tex-span">1 ≤ <i>dmg</i><sub class="lower-index"><i>i</i></sub> ≤ 2000</span>). </p>


## Output

<p>In case Petya can’t complete this level, output in the single line <span class="tex-font-style-tt">NO</span>.</p><p>Otherwise, output on the first line <span class="tex-font-style-tt">YES</span>. On the second line output the minimal time after which the boss can be defeated and the number of used scrolls. In the next lines for each used scroll output space-separated number of seconds passed from the start of the battle to the moment the scroll was used and the number of the scroll. Scrolls are numbered starting from 1 in the input order. The first scroll is considered to be available to be used after <span class="tex-span">0</span> seconds.</p><p>Output scrolls in the order they were used. It is not allowed to use scrolls after the boss is defeated.</p>


## Samples

```input1
2 10 3
100 3
99 1

```

```output1
NO

```






```input2
2 100 10
100 11
90 9

```

```output2
YES
19 2
0 1
10 2

```



