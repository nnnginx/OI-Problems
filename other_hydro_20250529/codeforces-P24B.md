## Description

<div><p>Formula One championship consists of series of races called Grand Prix. After every race drivers receive points according to their final position. Only the top 10 drivers receive points in the following order 25, 18, 15, 12, 10, 8, 6, 4, 2, 1. At the conclusion of the championship the driver with most points is the champion. If there is a tie, champion is the one with most wins (i.e. first places). If a tie still exists, it is chosen the one with most second places, and so on, until there are no more place to use for compare.</p><p> Last year another scoring system was proposed but rejected. In it the champion is the one with most wins. If there is tie, champion is the one with most points. If a tie still exists it is proceeded the same way as in the original scoring system, that is comparing number of second, third, forth, and so on, places.</p><p>You are given the result of all races during the season and you are to determine the champion according to both scoring systems. It is guaranteed, that both systems will produce unique champion.</p></div><div class="input-specification"><p>The first line contain integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 20</span>), where <span class="tex-span"><i>t</i></span> is the number of races. After that all races are described one by one. Every race description start with an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) on a line of itself, where <span class="tex-span"><i>n</i></span> is the number of clasified drivers in the given race. After that <span class="tex-span"><i>n</i></span> lines follow with the classification for the race, each containing the name of a driver. The names of drivers are given in order from the first to the last place. The name of the driver consists of lowercase and uppercase English letters and has length at most 50 characters. Comparing of names should be case-sensetive.</p></div><div class="output-specification"><p>Your output should contain exactly two line. On the first line is the name of the champion according to the original rule, and on the second line the name of the champion according to the alternative rule.</p></div>


## Input

<p>The first line contain integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 20</span>), where <span class="tex-span"><i>t</i></span> is the number of races. After that all races are described one by one. Every race description start with an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 50</span>) on a line of itself, where <span class="tex-span"><i>n</i></span> is the number of clasified drivers in the given race. After that <span class="tex-span"><i>n</i></span> lines follow with the classification for the race, each containing the name of a driver. The names of drivers are given in order from the first to the last place. The name of the driver consists of lowercase and uppercase English letters and has length at most 50 characters. Comparing of names should be case-sensetive.</p>


## Output

<p>Your output should contain exactly two line. On the first line is the name of the champion according to the original rule, and on the second line the name of the champion according to the alternative rule.</p>


## Samples

```input1
3
3
Hamilton
Vettel
Webber
2
Webber
Vettel
2
Hamilton
Vettel

```

```output1
Vettel
Hamilton

```






```input2
2
7
Prost
Surtees
Nakajima
Schumacher
Button
DeLaRosa
Buemi
8
Alonso
Prost
NinoFarina
JimClark
DeLaRosa
Nakajima
Patrese
Surtees

```

```output2
Prost
Prost

```




## Note

<p>It is not guaranteed that the same drivers participate in all races. For the championship consider every driver that has participated in at least one race. The total number of drivers during the whole season is not more then <span class="tex-span">50</span>.</p>

